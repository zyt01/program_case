# 修改函数上下文
- 对象

---
```JavaScript
function changeColor(color) {
    this.style.color = color;
}

changeColor("white");//failed

var main = document.getElementById("main");

changeColor.call(main, "red");

function setBodyColor() {
    changeColor.apply(document.body, arguments);
}

setBodyColor("green");
```
