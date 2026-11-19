# Project Overview
مشروع عبارة عن أداة بسيطة لفحص المنافذ (Port Scanner) باستخدام لغة Python، تسمح للمستخدم بإدخال عنوان IP أو اسم المضيف (Hostname)، ثم محاولة الاتصال بمجموعة من المنافذ المحددة لمعرفة المنافذ التي تستقبل اتصالات TCP.
# Objective
- تعلم بناء أداة بسيطة لفحص المنافذ باستخدام Python.
- التحقق من صحة عدد المدخلات باستخدام sys.argv.
- تحويل اسم المضيف إلى عنوان IPv4.
- التعرف على المنافذ المفتوحة من خلال اختبار الاتصال بها.
- التعامل مع الأخطاء أثناء تشغيل البرنامج
# Requirements
- انشاء ملف فحص على عنوان IP ومعرفة المنافذ المفتوحة التي يمكن استغلالها 
# Concepts Used
- SYS : للتعامل مع نظام تشغيل بايثون
- Socket : لإنشاء اتصالات الشبكة والتعامل مع عناوين IP والمنافذ
- Datetime : لاجل معرفة التاريخ والوقت الذي تمت به المهمة 
- IF Statements : لاجل تنفيذ من دون اخطاء والمشي على الشروط المطلوبة
- FOR Loop : لاجل فحص المنافذ كلها من امر واحد
- Except : لتبين حدوث اخطاء من ماذا 
# Implementation
```
import sys
import socket
from datetime import datetime
```
يستخدم هذا الجزء لاستيراد المكتبات التي يحتاجها البرنامج:

- sys: للتعامل مع مدخلات البرنامج وإنهائه.
- socket: لإنشاء اتصالات الشبكة وفحص المنافذ.
- datetime: للتعامل مع التاريخ والوقت وتسجيل توقيت تنفيذ البرنامج.

```
if len(sys.argv) == 2 : 
	target = socket.gethostbyname(sys.argv[1]) # Translater hostname to IPv4
else:
	print ("invalid arguments")
	print ("Syntax: python3 scanner.py ip")
```
يستخدم هذا الجزء للتحقق من عدد المدخلات التي يدخلها المستخدم عند تشغيل البرنامج باستخدام sys.argv ، فإذا كان عدد العناصر يساوي 2، يأخذ المدخل الأول من المستخدم ويحوّله إلى عنوان IPv4 باستخدام socket.gethostbyname() ويحفظه في المتغير target
أما إذا كان عدد المدخلات غير صحيح، فيطبع رسالة خطأ ويوضح طريقة تشغيل البرنامج الصحيحة

```
print ("Your IP is : " + target)
print ("Time Started : " +str(datetime.now()))
```
يستخدم هذا الجزء print() لعرض عنوان IP المستهدف والمخزن في المتغير target، ثم يعرض وقت بدء عملية الفحص باستخدام datetime.now().
تُستخدم str() لتحويل قيمة التاريخ والوقت إلى نص (String) حتى يمكن دمجها مع النص وطباعتها.

```
try:
	for port in range(50,58)
		soc = socket.socket(socket.AF_INET , socket.SOCK_STREAM)
		socket.setdefaulttimeout(1)
		result = soc.connect_ex((target , port))
		if result == 0:
			print(f"Port {port} is OPEN ")
		soc,close()
```
يستخدم هذا الجزء حلقة for لفحص مجموعة من المنافذ باستخدام range()، حيث يتم إنشاء Socket لكل منفذ باستخدام IPv4 وTCP.
بعد ذلك، يتم تحديد مهلة الاتصال باستخدام setdefaulttimeout()، ثم محاولة الاتصال بالمنفذ باستخدام connect_ex() وحفظ النتيجة في المتغير result.
إذا كانت النتيجة تساوي 0 فهذا يعني نجاح الاتصال وأن المنفذ مفتوح (OPEN)، وبعد الانتهاء يتم إغلاق الـ Socket باستخدام close().

```
except KeyboardInterrupt:
	print("\nYou exit the program")
	sys.exit()
except socket.gaierror:
	print("Hostname is not defined")
	sys.exit()
except socket.error:
	print("A Server error occurred")
	sys.exit()
```
يستخدم هذا الجزء except لمعالجة الأخطاء المحتملة أثناء تشغيل البرنامج، ويحتوي على ثلاثة أنواع:
- KeyboardInterrupt: التعامل مع إيقاف البرنامج يدوياً باستخدام Ctrl + C.
- socket.gaierror: التعامل مع أخطاء ترجمة اسم المضيف (Hostname) إلى عنوان IP.
- socket.error: التعامل مع أخطاء الاتصال المتعلقة بالـ Socket.
تُستخدم sys.exit() لإنهاء البرنامج بعد ظهور رسالة الخطأ المناسبة للمستخدم.
# Testing
```
#!/bin/python3

import sys
import socket
from datetime import datetime

if len(sys.argv) == 2 : 
	target = socket.gethostbyname(sys.argv[1]) # Translater hostname to IPv4
else:
	print ("invalid arguments")
	print ("Syntax: python3 scanner.py ip")

print ("-" * 50)
print ("Your IP is : " + target)
print ("Time Started : " +str(datetime.now()))
print ("-" * 50)

try:
	for port in range(50,85):
		soc = socket.socket(socket.AF_INET , socket.SOCK_STREAM)
		socket.setdefaulttimeout(1)
		result = soc.connect_ex((target , port))
		if result == 0:
			print(f"Port {port} is OPEN ")
		soc.close()

except KeyboardInterrupt:
	print("\nYou exit the program")
	sys.exit()
except socket.gaierror:
	print("Hostname is not defined")
	sys.exit()
except socket.error:
	print("A Server error occurred")
	sys.exit()
```
%%
python3 scanner.py 192.168.0.0
--------------------------------------------------
Your IP is : 192.168.0.0
Time Started : 2026-11-16 12:27:52.047198
--------------------------------------------------
Port 53 is OPEN 
Port 80 is OPEN 
%%
# Challenges
- فهم طريقة عمل sys.argv والتحقق من المدخلات.
- فهم كيفية إنشاء Socket والاتصال بالمنافذ.
- التمييز بين المنفذ المفتوح وفشل الاتصال
- التعامل مع الأخطاء باستخدام try و except
# What I Learned
- كيفية استخدام مكتبات Python في مشاريع الشبكات.
- كيفية التعامل مع عناوين IP و Hostname.
- كيفية إنشاء اتصال TCP باستخدام Socket.
- كيفية فحص مجموعة من المنافذ باستخدام For Loop.
- كيفية اكتشاف أخطاء الاتصال ومعالجتها.