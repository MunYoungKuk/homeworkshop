# Homework 19

## 1.

- CSRF(Cross-site request forgery)

## 2.

```python
def create(request):
    title = request.POST.get("title")
```

## 3.

```html
<form action="/posts/{{post.id}}/update" method="post">
    {% csrf_token %}
    <input type="text" name="title" value= "{{post.title}}">
    <input type="text" name="content" value = "{{post.content}}">
    <input type="submit" value="Submit"
</form>
```





