## ==Lab 1==
---
### **Escape Sequences Characters**
---
- في قوقل  Python Escape Sequences List فيها جميع المعلومات 

- \b => Back Space
	احذف الحرف القبلها
```
print ("Hello\bword")
```
- \newLine => Espace New Line
	في حال اكمال الطباعة في سطر جديد 
```
print ("Hello \
my name \
is mizu")
```
- \ => Escape Back Slash
	يحذف ما بعدها 
```
print ("My Name Is Mizu \\")
```
- \\' - \\" => Escape Single - Double Quote
	لاظهار علامة التنصيص في الرسالة
```
print ("My Name Is \'Mizu\'")
print ("My Name Is \"Mizu\"")
```
- \n => New Line
	ينزل سطر جديد
```
print ("My Name\nIs Mizu")
```
- \t => Horizontal Tab
	يجعل مسافة Tab في مكانها
```
print("My Name\tIs Mizu")
```
---
## ==Lab 2==
---
### **Concatenation**
---
- هي عميلة ربط الاسترنج ببعضها
```
A = "Hello "
B = "Word"
print (A + B)
```
- لا يمكن ربط استرينج مع ارقام
```
print ("Hello" + 1) => Error
```