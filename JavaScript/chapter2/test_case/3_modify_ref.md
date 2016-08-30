# 修改对象的引用，同时保持完整性
- 对象
- 引用
- 数组

---
```JavaScript
var items = new Array("one", "two", "three");

var itemsRef = items;

items = new Array("new", "array");

console.log(items != itemsRef);
```
