 Например, вот как быстро получить свой текущий внешний IP:

```
$ curl ifconfig.me
93.96.141.93
```

Параметры -i (показывать заголовки) и -I (показывать только заголовки) делают cURL отличным инструментом для дебаггинга HTTP-ответов и анализа того, что конкретно сервер вам отправляет:

```
$ curl -I habrahabr.ru
HTTP/1.1 200 OK
Server: nginx
Date: Thu, 18 Aug 2011 14:15:36 GMT
Content-Type: text/html; charset=utf-8
Connection: keep-alive
Keep-alive: timeout=25
```

Параметр -L тоже полезный, он заставляет cURL автоматически следовать по редиректам. cURL поддерживает HTTP-аутентификацию, cookies, туннелирование через HTTP-прокси, ручные настройки в заголовках и многое, многое другое.