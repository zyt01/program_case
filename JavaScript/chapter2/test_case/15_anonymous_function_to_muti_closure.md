# 使用匿名函数来激发出创建多个使用闭包的函数所需的作用域
- 作用域
- 闭包

---
```JavaScript
var obj = document.getElementById("main");

var items = ["click", "keypress"];

for (var i = 0; i < items.length; i++) {
    (function() {
        var item = items[i];

        obj["on" + item] = function() {
            alert("Thanks for your " + item);
        };
    });
}
```
