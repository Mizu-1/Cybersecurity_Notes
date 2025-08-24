## ==Lab 1==
---
### **Variables المتغيرات**
---
#### **part 1**

طريقة كتابة المتغيرات :
{ اسم المتغير - علامة اساوي - المتغير }
```
`MyVariable = " MyVariable "`
`print (MyVariable)`
```

قوانين في كتابة المتغيرات :
- تقدر ان يبداء المتغير ب a -z , A - Z , _
```
`MyVariable = " MyVariable "`
`print (MyVariable)`

`myVariable = " MyVariable "`
`print (myVariable)`

`_MyVariable = " MyVariable "`
`print (_MyVariable)`
```
- ما تقدر ان يبداء المتغير بارقام او علامة مميزة
```
`100MyVariable = " MyVariable "`
`print (100MyVariable)`
```
- تقدر ان تضع ارقام او شرطة سفلية في وسط المتغير
```
`My55Variable = " MyVariable "`
`print (My55Variable)`

`My_Variable = " MyVariable "`
`print (My_Variable)`
```
- ما تقدر ان تضع علامة خاصة في وسط المتغير
```
`My-Variable = " MyVariable "`
`print (My-Variable)`

`My@Variable = " MyVariable "`
`print (My@Variable)`
```
- في الطباعة يجب ان تتشابة الحروف لا يمكن وضع حرف كبير في المتغير وتضعه صغير في الطباعة
```
`MyVariable = " MyVariable "`
`print (myVariable)`
```
- لاتقدر ان تطبع المتغير قبل كتابة المتغير
```
`print (MyVariable)`
`MyVariable = " MyVariable "`
```
- تسمة المتغيرات :
```
Name = "Mizu" # Singel Word => Normal
myName = "Mizu" # Tow Word => CamelCase
My_Name = "Mizu" # Tow Word => Snake_Case
```

---
#### **part 2**

- Source Code : هو اي سطر كود برمجي في اي لغة او بمسمى اخر كود طبيعي
- Translation : هي عملية تحويل او ترجمة الكود للالة
- Compilation : Run Time هي عملية ترجمة للكود قبل
- Run Time : هي المدة المستقرقة لتنفيذ الكود
- Interpteted : هي عملية ترجمة للكود اثناء تشغيل الاوامر

- في لغة بايثون يمكن تغير قيمة المتغير اثناء تشغيل الكود :
```
x = 10
x = "hello"

print (x)
```
- طريقة معرفة الكلمات المحجوزة :
```
help ("keywords")
```
- طريقة كتابة اكثر من متغير مع قيمهم :
```
a, b, c = 1, 2, 3
print (a)
print (b)
print (c)
```