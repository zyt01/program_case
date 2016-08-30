# 使用匿名函数来隐藏全局作用域变量
- 作用域
- 闭包

---
```JavaScript
(function() {
    var msg = "Thanks for visiting!";

    window.onunload = function() {
        alert(msg);
    };
})();
```
