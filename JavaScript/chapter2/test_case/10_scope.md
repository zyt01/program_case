# 变量作用域
- 作用域

---
```JavaScript
var foo = "test";

if (true) {
    var foo = "new test";
}

console.log(foo);

function test() {
    var foo = "old test";
}

test();

console.log(foo);
```
