# 在上下文对象内使用函数并将其上下文对象切换为另一个变量
- 对象

---
```JavaScript
var obj = {
    yes: function() {
        this.val = true;
    },
    no: function() {
        this.val = false;
    }
};

console.log(obj.val);

obj.yes();

console.log(obj.val);

window.no = obj.no;
window.no();

console.log(obj.val);

console.log(window.val);
```
