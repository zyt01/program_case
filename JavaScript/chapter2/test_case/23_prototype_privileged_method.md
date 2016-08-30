# 使用特权方法
- 对象
- 原型
- 方法

---
```JavaScript
function User(name, age) {
    var year = (new Date()).getFullYear() - age;

    this.getYearBorn = function() {
        return year;
    }
}

var user = new User("Bob", 44);

console.log(user.getYearBorn());

console.log(user.year);
```
