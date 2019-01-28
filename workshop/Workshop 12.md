# Workshop 12

```python
#workshop12.py
from flask import Flask, render_template
app = Flask(__name__)

@app.route("/")
def hello():
    return "Hello World!"
    
    
@app.route("/grid")
def grid():
    return render_template("grid.html")

if __name__ == "__main__":
    app.run(debug=True,host='0.0.0.0',port='8080')
```



```html
<--!grid.html-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css" integrity="sha384-GJzZqFGwb1QTTN6wy59ffF1BuGJpLSa9DkKMp0DgiMDm4iYMj70gZWKYbI706tWS" crossorigin="anonymous">
</head>
<body>
    <div class = "container">
        <div class ="row">
            <div class= "col border bg-danger rounded border-dark col-xl-3 col-md-6 col-12"><p>1</p></div>
            <div class= "col border bg-danger rounded border-dark col-xl-3 col-md-6 col-12"><p>1</p></div>
            <div class= "col border bg-danger rounded border-dark col-xl-3 col-md-6 col-12"><p>1</p></div>
            <div class= "col border bg-danger rounded border-dark col-xl-3 col-md-6 col-12"><p>1</p></div>
            
        </div>    
    </div>
</body>
</html>
```

