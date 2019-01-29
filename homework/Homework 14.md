# Homework 14

## 1.

```python
ALLOWED_HOSTS = ["*"]
```

## 2.

```python
def index(request):
    posts = Post.objects.order_by('-id').all()
    return render(request, "ssafy/index.html", {"posts":posts})
```

## 3.

```powershell
python manage.py runserver $IP:$PORT
```

## 4.

Model, Template, View