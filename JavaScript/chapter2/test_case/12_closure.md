# 闭包
- 作用域
- 闭包

---
```JavaScript
var obj = document.getElementById("main");

obj.style.border = "1px solid red";

setTimeout(function(){
    obj.style.display = "none";
}, 1000);

function delayedAlert(msg, time) {
    setTimeout(function(){
        alert(msg);
    }, time);
}

delayedAlert("Welcome!", 2000);
```
