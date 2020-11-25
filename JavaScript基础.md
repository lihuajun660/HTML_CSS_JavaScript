JavaScript基础
===============
1. 一种真正的编程语言，可以在网页上实现复杂的功能交互
2. 解释型语言（不需要预先编译）
3. 运行在客户端（跑在浏览器上的）
4. 面向对象语言

原名：LiveScript->>JavaScript蹭Java热度

三种方式添加JavaScript
---------------
1. 内部的JavaScript 
  <script>
  </script>
2. 外部的JavaScript
  <script src = "script.js"> </script>
3. 内联JavaSript(**X**)不推荐
  <button onclick = "createPrargraph()">
  Click me
  </button>
  
类型、对象、变量、数组、运算符、函数、控制结构、闭包
----------------------
1. 所有数字都使用浮点数类型，double双精度
2. alert();
```
<script>

</script>
````

3. console.log，来显示

```JavaScript
console.log("Hello".length);

console.log("hello".charAt(2));

console.log("hello, world".replace("hello", "goodbye"));

console.log("hello, world".toUpperCase);
```

* &&, ||
* var, let, const
	* var可以在任何地方进行访问
	* let的作用域只在代码块中{}
* while, do...while...同Java
* for循环
* 三目运算符：var allowed = age >= 18 ?  "Yes":"No";
* switch(a){case 1: {}}
* Object
```JavaScript
var obj = new Object();
var obj2 = {};

obj = {
    name : "Simon",
    age : '20',
    email : "simon@gmail.com",
    contact: { 
        phone: "12345667",
        Telegram: "@Simon"
    }
}


console.log(obj["contact"]["phone"]);
```

数组
------------
var a = new Array();
for (let i = 0; i < a.length; i++){
}

变种for循环：
for (let i in a){}---->只会访问其中有值的部分
pop(),reverse(),shift()--->删除第一个元素
unshift()--->在数组第一个位置加入元素
 
 
arguments--->指代传入参数的一个集合
-----------
```
function add(){
    let sum = 0;
    for (let i = 0, j = arguments.length; i< j;i++){
        sum += arguments[i];
    }
    return sum;
}

let a = add(1,2,3,4,54,65);

console.log(a);
```

闭包
--------
```JavaScript
function makeAdder(a, b){
    return function(b){
        return a + b;
    }
}

var x = makeAdder(6);
//相当于返回了一个函数赋值给了x， 此后的x就作为一个函数来用了。
var sum = x(2);
console.log(sum);

```
