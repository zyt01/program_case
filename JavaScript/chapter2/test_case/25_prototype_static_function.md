# 静态方法例子
- 对象
- 原型
- 方法

---
```JavaScript
User.cloneUser = function() {
    return new User(
        user.getName(),
        user.getAge()
    );
};

```
