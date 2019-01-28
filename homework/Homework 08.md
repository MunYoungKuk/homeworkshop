# Homework 08 -190116

## 1번

### (a) : request(요청)

### (b) : response(응답)



## 2번

```python
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello():
    return "Hello World!"
```

```bash
$ pip install Flask
$ FLASK_APP=hello.py flask run
```



## 3번

```python
from flask import Flask
```



## 4번

```bash
$ FLASK_APP=app.py flask run --host=$IP --port=$PORT
```

