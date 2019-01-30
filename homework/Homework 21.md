# Homework 21

## 1.

```html
{% for comment in question.comment_set.all %}
	<h3>{{comment.content}}</h3>
{% endfor %}
```

## 2.

```html
<form action="/questions/{{question.id}}/comments/create/" method="post>
```

