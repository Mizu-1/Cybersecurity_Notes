معناها **استيراد الوحدات أو المكتبات**.
ببساطة: أحيانًا نحتاج إلى استخدام أوامر ووظائف جاهزة في بايثون، فنستوردها بدلًا من كتابة كل شيء بأنفسنا.
```
import sys #system functions and parameters
print(sys.version)
```
هذا المثال يشرح استخدام مكتبة sys في بايثون.
```
from datetime import datetime as dT
print (dT.now())
```
هذا المثال يشرح استيراد دالة التاريخ والوقت من مكتبة datetime باستخدام from و as.
`from datetime`: استيراد شيء من مكتبة `datetime`.
`import datetime`: استيراد الكلاس `datetime` الموجود داخل المكتبة.
`as dT`: إعطاء اسم مختصر له وهو `dT`.
`dT.now()`: الحصول على التاريخ والوقت الحاليين.
`print()`: طباعة النتيجة.