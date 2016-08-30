# 只能由构造函数访问的私有方法
- 对象
- 原型
- 方法

---
```JavaScript
function Classroom(students, teacher) {
    function disp() {
        console.log(this.students.join(", "));
    }

    this.students = students;
    this.teacher = teacher;

    disp();
}

var _class = new Classroom(["John", "Bob"], "Mr. Smith");

_class.disp(); //failed
```
