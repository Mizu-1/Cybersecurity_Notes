الجمل الشرطية هي عبارة عن تحقيق الشروط لاكتمال الكود او الوصول للمطلوب
```
def buydrink(money):
	if money >= 50:
		return "you can buy the drink"
	else:
		return "you can`t buy the drink"
print (buydrink(25))
print (buydrink(51))
```
في هذا المثال في حال كان مبلغ العميل اكثر من 51 يطبع له "يمكنك شراء المشروب"
واذا كان اقل يطبع له "لا يمكنك شراء المشروب"

هذا مثال بسيط لعمل الجمل الشرطية في بايثون
```
def placerules(age,money):
	if (age >= 21) and (money >= 1000):
		return "you can allowed to enter"
	elif (age >= 21) and (money < 1000):
		return "you need a money = 1000$"
	elif (age < 21) and (money >= 1000):
		return "your age is not allowed"
	else:
		return "you can`t allowed to enter"
print (placerules(24,300))
```
هذا مثال ايضا للجمل الشرطية لا يمكن دخول المكان الا بعد تحقيق الشروط العمر 21 او اكبر المال 1000 او اكثر
