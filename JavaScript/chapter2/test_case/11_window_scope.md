# 全局作用域和 window 对象
- 作用域
- 全局

---
```JavaScript
var test = "test";

console.log(window.test === test);


function testFoo() {
    foo = "test";
}

testFoo();

console.log(window.foo === "test");
```
