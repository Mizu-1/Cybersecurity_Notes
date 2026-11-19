في هذا الدرس سنتعرف على مفهوم **Classes and Objects** في لغة Python، وكيفية استخدام البرمجة الكائنية (Object-Oriented Programming - OOP) لتنظيم الكود وإنشاء كائنات تحتوي على بيانات وخصائص ودوال خاصة بها.
سنتعلم كيفية إنشاء Class، وإنشاء Objects منه، والتعامل مع الخصائص والدوال داخل الكائنات، مع تطبيق أمثلة عملية لفهم الفكرة.
```
class Emp:
	def __init__(self , name , salary , number_of_years_exp , field):
		self.name = name
		self.salary = salary
		self.number_of_years_exp = number_of_years_exp
		self.field = field
```

```
#!/bin/python3

from emp import Emp
emp1 = Emp("mizu" , 9000 , 3 , "cs")
print (emp1.salary)

```
في هذا المثال أنشأنا Class باسم Emp يحتوي على خصائص الموظف مثل الاسم والراتب وسنوات الخبرة والتخصص.
- `__init__`: دالة يتم تشغيلها تلقائياً عند إنشاء كائن جديد.
- `self`: تشير إلى الكائن نفسه، وتُستخدم لتخزين واستدعاء خصائصه.
- `self.name` وغيرها: تمثل الخصائص التي يحتفظ بها كل كائن.
في الملف الثاني استوردنا Emp باستخدام from emp import Emp، ثم أنشأنا كائناً باسم emp1 وأرسلنا إليه بيانات الموظف.
وأخيراً استخدمنا emp1.salary لاستدعاء راتب الموظف.
**الخلاصة:** الـ Class هو القالب الذي نُنشئ منه Objects، وكل Object يمتلك بياناته الخاصة بناءً على هذا القالب.