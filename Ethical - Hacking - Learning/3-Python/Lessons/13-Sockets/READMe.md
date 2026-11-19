هو طريقة لاتصال جهازين عن طريق المنافذ وعناوين ip

```
import socket
host = '127.0.0.1'
port = 7777

soc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
# AF_INET = IPv4 , SOCK.STREAM = port
soc.connect((host , port))
```
في هذا الكود طريقة ربط المضيف بالمنفذ وطريقة الربط هنا انعمل بنفسي
```
nc -nvlp 7777
```
استحدمنا امر netcat لعمل عملية استماع للمنفذ بهذه الطريقة