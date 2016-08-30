# 用闭包实现的函数 curry 化
- 作用域
- 闭包

---
```JavaScript
function addGenerator(num) {
    return function(toAdd) {
        return num + toAdd;
    };
}

var addFive = addGenerator(5);

console.log(addFive(4));
```
