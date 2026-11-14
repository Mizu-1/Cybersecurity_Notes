
 البوليان Boolean في Python هو نوع من أنواع البيانات (Data Types)، ويُستخدم للتعبير عن حالتين فقط:

- `True` = صحيح
- `False` = خطأ
```
boolean1 = 3 + 4 == 7 #True
boolean2 = 3 + 6 == 5 #False

print (boolean1 , boolean2)
```
هذا مثال بسيط يوضح طريقة عملها
```
greaterthan = 10 > 6 #True
lessthan = 6 < 10 #True
greaterthanequal = 10 >= 10 #True
lessthanequal = 10 <= 10 #True
print (greaterthan , lessthan , greaterthanequal , lessthanequal)
```
هذا مثال اخر للBoolean
```
Op1 = (10 > 6) and (10 < 10) #Falde
Op2 = (10 > 6) and (10 <= 10) #True
Op3 = (10 > 6) or (10 < 10) #True
Op4 = (10 < 6) or (10 < 10) #False
print (Op1 , Op2 , Op3 , Op4)
```
في هذا المثال استخدمت الand و or 
الand هي اذا كان الشرطين صحيحين يطبع صحيح وباقي الاحتمالات خطأ
الor اذا كان احد الشرطين او كلاهما صحيح يطبع صحيح وباقي الاحتمالات خطأ