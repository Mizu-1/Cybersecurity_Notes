في هذا الدرس سوف نتعمق في السلاسل النصية String 
يمكن انقذ اوامر القائمات lists فيها 
```
name = "ahmed"
print (name)
print (name[0]) # first letter
print (name[-1]) # Last letter
```

```
CN = "Mizu 111"
print (CN[:4]) # عرض الاحرف من الاول الى الحرف الرابع
print (CN.split()) # جعلها في لست بين كل فراق عنصر
```

```
X = ["ahmed" , "ali" , "omar"]
print (X)
print (" ".join(X))
```
هذا الامر يستخرج القائمة ويطبعها بشكل طبيعي بدون اقواس او فواصل
```
test = "my chanel name is 'MR.Mizu'"
print (test)
test2 = 'my chanel name is "MR.Mizu"'
print (test2)
```
هذا الامر يطبع السينقل كود داخل الدابل كود او العكس (لا يمكن ادخال السينقل كود داخل السينقل كود او العكس للدابل كود)
```
test3 = 'my chanel name is \'MR.Mizu\''
print (test3)
```
هذه الطريقة التي يمكن طباعة سينقل كود داخل سينقل كود او في الدابل كود ايضا 
```
hello = "          hello         "
print (hello)
print (hello.strip())
```
هذا الامر يحذف المسافات التي قبل وبعد الكلمة في الطابعة
```
print ("A" in "Ahmed") # true
print ("a" in "Ahmed") # false
```
 الحروف في لغة بايثون حساسة يفرق الحروف الكبيرة عن الصغيرة
```
L = "AHmed"
print (L.lower())
print (L.())
```
هذا الامر يحول الحروف الكبيرة الى صغيرة
```
x = "Mr.Mizu"
print ("My Channel Name Is: " + x)
print ("My Channel Name Is: {}".format(x))
print ("My Channel Name Is: %s"%x)
print (f"My Channel Name Is: {x}")
```
هذه الاوامر لعمل توصيل النص مع المتغيير والطريقة الاخيرة هي الاحدث في لغة بايثون