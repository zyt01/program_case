# 多个变量引用同一个对象
- 对象
- 引用

---
```JavaScript
var obj = new Object();

var objRef = obj;

obj.oneProperty = true;

console.log(obj.oneProperty === objRef.oneProperty);
```
