# 修改对象而生成新对象
- 对象
- 引用
- 字符串

---
```JavaScript
var items = "test"

var itemsRef = items;

items += "ing"

console.log(items != itemsRef);
```
