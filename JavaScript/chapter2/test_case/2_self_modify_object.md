# 自修改对象的例子
- 对象
- 引用
- 数组

---
```JavaScript
var items = new Array("one", "two", "three");

var itemsRef = items;

items.push("four");

console.log(items.length === itemsRef.length);
```
