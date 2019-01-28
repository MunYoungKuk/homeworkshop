# Workshop 10

## 1번

```html

<style>
    #ssafy > p:nth-child(2) {
        color : red;
    }
</style>
<div id = "ssafy">
    <h2>어떤게 선택될까?</h2>
    <p>첫번째 단락</p>
    <p>두번째 단락</p>
    <p>세번째 단락</p>
    <p>네번째 단락</p>  
</div>
```

- p:nth-child()를 사용하였을때는 다 포함하여 순서대로 찾지만 p:nth-of-type()은 p를 찾는다.