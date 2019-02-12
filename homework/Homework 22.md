# Homework 22

## 1.

```python
class Post(models.Model):
    attachment = models.FileField
```

## 2.

```python
MEDIA_URL = '/uploaded_files/' # 항상 / 로 끝나도록 설정
# MEDIA_URL = 'http://static.myservice.com/media/' 다른 서버로 media 파일 복사시

# 업로드된 파일을 저장할 디렉토리 경로
MEDIA_ROOT = os.path.join(BASE_DIR, 'uploaded_files')
```

## 3.

```python
STATICFILES_DIRS =[
  os.path.join(BASE_DIR,"assets")
]
```

