# 维护传入函数的所有参数
- 函数
- 类型
- 参数

---
```JavaScript
function strict(types, args) {
    if (types.length != args.length)
        throw "Invalid number of arguments. Expected " + types.length +
        ", received " + args.length + " instead.";

    for (var i = 0; i < args.length; i++)
        if (args[i].constructor != types[i])
            throw "Invalid argument type. Expected " + types[i].name +
            ", received " + args[i].constructor.name + " instead.";
}

function userList(prefix, num, users) {
    strict([String, Number, Array], arguments);

    for (var i = 0; i < num; i++)
        console.log(prefix + ": " + users[i]);
}
```
