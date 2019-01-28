# Workshop 08

```python
#app.py

from flask import Flask, render_template
app = Flask(__name__)

a= {'apple':"사과",'grape':"포도",'watermelon':"수박",'banana':"바나나"}

@app.route("/dictionary/<string:word>")
def my_dict(word):
    if word in a.keys():
        return render_template("dictionary.html",word=word ,words=a.get(word))
    else:
        return f"{word}은(는) 나만의 단어장에 없는 단어 입니다."
        
if __name__ == "__main__":
    app.run(debug=True,host='0.0.0.0',port='8080')
```



```html
<--!dictionary.html-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>workshop08</title>
</head>
<body>
    <h1>{{word}}은(는) {{words}}</h1>
</body>
</html>
```

