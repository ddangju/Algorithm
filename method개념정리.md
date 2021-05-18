# 개념정리

---
<br>

### String.prototype.split()

***String*** 객체를 여러 개의 문자열로 나누고 array로 반환된다

빈 문자열이 주어졌을 경우 ```split()```은 빈 배열이 아니라 빈 문자열을 포함한 배열을 반환한다. 

<br>

```jsx
const string = ""
const split = string.split();

console.log(split); /// [" "]
```

