# 显示错误信息和默认信息
- 类型
- 函数

---
```JavaScript
function displayerror(msg) {
    if (typeof msg === "undefined")
        msg = "An error occurred.";

    console.log(msg);
}
```
