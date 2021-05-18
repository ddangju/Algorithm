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

### Array.prototype.includes()

배열이 특정 요소를 포함하고 있는지 판별한다.
문자나 문자열을 비교할 때 *대소문자* 를 구분한다!
반환값은 boolean 값.

```jsx

const pets = ['cat', 'dog', 'bat'];

console.log(pets.includes('cat')); //ture
```

### Array.prototype.splice()

기존 배열을 *삭제 또는 교체* 하거나 새 요소를 *추가* 하여 배열의 내용을 변경한다.
