# 简单对象的创建和使用
- 对象
- 创建
- 使用

---
```JavaScript
function User(name) {
    this.name = name;
}

var me = new User("My Name");

console.log(me.name);

console.log(me.constructor);

User("Test");

console.log(window.name);
```
