# Workshop 21

## 1.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <h1>{{question.title}}</h1>
    {% for choice in question.choice_set.all %}
        <h3>{{choice.content}} : {{choice.votes}}</h3>
    {% endfor %}
</body>
</html>
```

