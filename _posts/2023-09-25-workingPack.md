---
layout : single
title : "일 할떄 자주 사용하는 것들 모음"
---

### 1. 숫자 표현 정규식 (1000 -> 1,000)
```js
var before = 1000;
var after = n.toString().replace(/\B(?<!\.\d*)(?=(\d{3})+(?!\d))/g, ",");
console.log(after); // 1,000
```
```java
int before = 1000;
DecimalFormat decimalFormat = new DecimalFormat("#,###");
String after = decimalFormat.format(x);
System.out.println(after); // 1,000
```
