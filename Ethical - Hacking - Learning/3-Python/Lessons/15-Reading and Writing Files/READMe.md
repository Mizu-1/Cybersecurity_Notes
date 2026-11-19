سنتعلم طريقة قراءة وكتابة الملفات في بايثون
عملنا مجموعة كلمات مرور داخل ملف عادي وقمنا باستدعاء الملف من بايثون بهذه الطريقة
```
passowrd = open("passowrd.txt")
print(passowrd)
passowrd.close()
```
`<_io.TextIOWrapper name='pass.txt' mode='r' encoding='UTF-8'>`
هذه مخرجات الكود ويهمنا من المخرجات المود
```
passowrd = open("passowrd.txt")

print(passowrd)
print(passowrd.mode) #r
print(passowrd.readable()) #True لمعرفة الملف قابل للقراءة او لا
passowrd.close()
```
هذه احد الطرق لمعرفة مود الملف اذا كان للقراءة او للكتابة او الاثنين
```
passowrd = open("passowrd.txt")

print(passowrd.read())

passowrd.close()
```
هذا الامر لقراءة محتويات الملف في بايثون
```
passowrd = open("passowrd.txt")

print(passowrd.readline())

passowrd.close()
```
هذا الامر لقراءة الملف سطر الاول اذا اريد السطر الثاني اكرر الامر مره اخرى
```
passowrd = open("passowrd.txt")

print(passowrd.readlines())

passowrd.close()
```
هذا الامر لقراءة الملف ويضعها داخل قائمة باضافة حرف s
```
data = open("dt.txt" , "w")
print(data)
data.close()
```
هذا الامر للانشاء ملف قابل للكتابة فيه ومعرفة نوعه
```
data = open("dt.txt" , "w")
data.write("this my data")
data.close()
```
هذا الامر تستطيع الكتابة داخل الملف
```
data = open("dt.txt" , "a")
data.write("\n another data")
data.close()
```
كذا تقدر تكتب اكثر من سطر مع تغيير حرف w الى a 