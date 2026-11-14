القاموس Dictionary هو نوع من أنواع تخزين البيانات في بايثون، يخزن المعلومات على شكل مفتاح وقيمة (Key & Value).
```
food = {"pizza" : 24 , "burger" : 15 , "shawarma" : 20}
print (food)
```
هذا مثال عليها تكون في اقواس { } 
```
emp = {"IT" : ["ahmed" , "ali"] , "cs" : ["mazen" , "mizu"] , "hr" : ["zead" , "osama"]}

emp ["wep"] = ["samy" , "ibrahem"]
print (emp)

emp.update({"sales" : ["ahmed", "abdo"]})
print (emp)
```
هذه الطرق لاضافة مفتاح وقيمة داخل القاموس
```
food = {"pizza" : 24 , "burger" : 15 , "shawarma" : 20}
print (food)

food["pizza"] = 30
print (food)
```
هذه الطريقة لتغيير القيمة المفتاح داخل القاموس
```
print (food.get("pizza"))
```
هذه الامر لاستدعاء قيمة المفتاح داخل القاموس