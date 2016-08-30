# 对象的方法通过 prototype 对象添加的例子
- 对象
- 原型
- 方法

---
```JavaScript
function User(name, age) {
    this.name = name;
    this.age = age;
}

User.prototype.getName = function() {
    return this.name;
}

User.prototype.getAge = function() {
    return this.age;
}

var user = new User("Bob", 44);

console.log(user.getName());
console.log(user.getAge());
```
