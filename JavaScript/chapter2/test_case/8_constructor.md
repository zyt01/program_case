# 使用构造函数属性来判断对象的类型
- 构造函数
- 类型

---
```JavaScript
if (num.constructor === String)
    num = parseInt(num);

if (str.constructor === Array)
    str = str.join(",");
```

---
### 变量检查

|变量|typeof 变量|变量.构造函数|
|-|-|-|
|{an:"object"}|object|Object|
|{an:"array"}|object|Array|
|function() {}|function|Function|
|"a string"|string|String|
|55|number|Number|
|true|boolean|Boolean|
|new User()|object|User|
