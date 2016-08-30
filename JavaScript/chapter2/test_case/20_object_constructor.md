# 使用 constructor 属性的例子
- 对象
- 创建
- 类

---
```JavaScript
function User() {}

var me = new User();

var you = new me.constructor();

console.log(me.constructor === you.constructor);
```
