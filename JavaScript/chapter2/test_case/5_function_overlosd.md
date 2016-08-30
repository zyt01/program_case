# 函数重载的两个例子
- 函数
- 参数

---
```JavaScript
function sendMessage(msg, obj) {
    if (arguments.length == 2)
        obj.handleMsg(msg);

    else
        console.log(msg);
}

sendMessage("Hello, World");

sendMessage("How are you?", {
    handleMsg: function(msg) {
        console.log("This is a custom massage: " + msg);
    }
});

function makeArray() {
    var arr = [];

    for (var i = 0; i < arguments.length; i++)
        arr.push(arguments[i]);

    return arr;
}
```
