## Run

``` python
python flask_basic.py
```

``` shell
curl -v http://127.0.0.1:5000

# print(app.url_map)
Map([<Rule '/' (HEAD, GET, OPTIONS) -> my_microservice>,
 <Rule '/static/<filename>' (HEAD, GET, OPTIONS) -> static>])

# print(request)
<Request 'http://127.0.0.1:5000/' [GET]>

# print(request.environ)
{'wsgi.version': (1, 0), 'wsgi.url_scheme': 'http', 'wsgi.input': <_io.BufferedReader name=14>, 'wsgi.errors': <_io.TextIOWrapper name='<stderr>' mode='w' encoding='UTF-8'>, 'wsgi.multithread': True, 'wsgi.multiprocess': False, 'wsgi.run_once': False, 'werkzeug.server.shutdown': <function WSGIRequestHandler.make_environ.<locals>.shutdown_server at 0x7fbc02be6598>, 'SERVER_SOFTWARE': 'Werkzeug/0.14.1', 'REQUEST_METHOD': 'GET', 'SCRIPT_NAME': '', 'PATH_INFO': '/', 'QUERY_STRING': '', 'REMOTE_ADDR': '127.0.0.1', 'REMOTE_PORT': 53354, 'SERVER_NAME': '127.0.0.1', 'SERVER_PORT': '5000', 'SERVER_PROTOCOL': 'HTTP/1.1', 'HTTP_HOST': '127.0.0.1:5000', 'HTTP_USER_AGENT': 'curl/7.61.1', 'HTTP_ACCEPT': '*/*', 'werkzeug.request': <Request 'http://127.0.0.1:5000/' [GET]>}

# print(response)
<Response 18 bytes [200 OK]>

# print(response.data)
b'{"Hello":"World"}\n'

```