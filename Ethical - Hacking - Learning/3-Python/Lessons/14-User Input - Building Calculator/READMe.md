في هذا الدرس سنتعلم ادخال البيانات من المستخدم وتخزينها او التعامل معها
```
input ("Enter your name: ")
input ("Enter your emali: ")
```
هذه طريقة جعل المستخدم يدخل البيانات
```
username = input ("Enter your name: ")
print("your namr is : "+ username)
```
هذه طريقة استخدام مدخلات المستخدم 
```
num1 = float(input("Enter Any Number: "))
opr = input("Enter Your Operator: ")
num2 =  float(input("Enter Any Number: "))

if opr == "+":
	print (num1 + num2)
elif opr == "-":
	print (num1 - num2)
elif opr == "*":
	print (num1 * num2)
elif opr == "/":
	print (num1 / num2)
elif opr == "**" or opr == "^":
	print (num1 ** num2)
else:
	print("Erorre")
```
هذا مشروع مصغر لالة حاسبة توضح طريقة جعل المستخدم يدخل بيانات والتعامل معها