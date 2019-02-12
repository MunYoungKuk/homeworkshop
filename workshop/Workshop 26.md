# Workshop 26

## 1.

```python
class StudentForm(forms.Form):
    name = forms.CharField(max_length=100)
    age = forms.IntegerField()
```

## 2.

```	html
{% extends "Student/base.html" %}

{% block bb %}
    <form method="post">
        {% csrf_token %}
        {{form}}
        <input type="submit" value="Submit"/>
        
    </form>
{% endblock %}
```

