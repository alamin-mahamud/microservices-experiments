## Run

``` python
python flask_basic.py
```

``` shell
curl -v http://127.0.0.1:5000

* Rebuilt URL to: http://127.0.0.1:5000/
*   Trying 127.0.0.1...
* TCP_NODELAY set
* Connected to 127.0.0.1 (127.0.0.1) port 5000 (#0)
> GET / HTTP/1.1
> Host: 127.0.0.1:5000
> User-Agent: curl/7.61.1
> Accept: */*
> 
127.0.0.1 - - [26/Feb/2019 21:52:37] "GET / HTTP/1.1" 200 -
* HTTP 1.0, assume close after body
< HTTP/1.0 200 OK
< Content-Type: application/json
< Content-Length: 18
< Server: Werkzeug/0.14.1 Python/3.7.1
< Date: Tue, 26 Feb 2019 15:52:37 GMT
< 
{"Hello":"World"}
* Closing connection 0
```