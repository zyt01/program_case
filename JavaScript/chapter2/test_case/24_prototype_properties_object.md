# 动态生成方法例子
- 对象
- 原型
- 方法

---
```JavaScript
function User(properties) {
    for (var i in properties) {(function(which){
        var p = i;
        which["get" + p] = function() {
            return properties[p];
        };

        which["set" + p] = function(val) {
            properties[p] = val;
        };
        })(this);
    }
}

var user = new User({
    name: "Bob",
    age: 44
});

console.log(user.name);

console.log(user.getname());

user.setage(22);

console.log(user.getage());
```
