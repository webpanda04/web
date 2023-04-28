<h1>JavaScript</h1>

# javascript基础

## Javascript 介绍

<ol>·ECMAscript:
  <p>
    规定了js基础语法核心知识。
  </p>
  </p></ol>


1. 规定了js基础语法核心知识。
2. 比如：变量，分支语句,循环语句，对象等等

web Apis：

1. DOM：操作文档，比如页面进行移动，大小，添加删除等操作

2. BOM ： 操作浏览器，比如弹窗，检测窗口宽度，存储数据浏览器等等

   

<img src="/Users/a123/Library/Application Support/typora-user-images/image-20230214090045061.png" alt="image-20230214090045061" style="zoom:50%;" />

## Javascript 输出和输入



​		console.log控制台打印

作用：控制台输出语法，程序员调试使用

```js
console.log("控制台")
```

​		aletr 弹出对话框输出

作用：页面弹出警告框

```javascript
aletr('弹出对话框')
```

document.write 文档输出

作用：向body内输出内容

注意：如果输出的内容写的是标签，也会被解析成网页元素

```js
document.write("输出内容")
```

### 输入

prompt("请输入你的age：")

作用：显示一个对话框，对话中包括文字信息，用来提示用户输入文字

```js
prompt("请输入你的age：")
```

## 字面量

在计算机科学中，字面量（literal）是计算机中描述 事/物

比如：

1.我们工资是：1000 此时 1000 就是  数字字面量

2.<b>"前端开发"</b>  字符串字面量

3.还有{}对象字面量 和 []数组字面量

<hr></hr>



# 变量

Let 和var 的区别：

var：可以先使用在声明，变量可以重复声明，比如变量提升，全局变量，没有块级作用域等等！（不合理，不规范）

let 出现的原因，弥补var的不足和不合理。



变量是什么？

- 白话：变量是装东西的盒子
- 通俗：变量是计算机中的存储数据的"容器"，它可以让计算机变得有记忆。
- 注意：变量本身不是数据，仅是存储的一个容器。可以理解是存储东西的

## 变量命名规范与规范

- 必须遵守，不遵守（法律层面）
- 规范：建议，不遵守不报错，但不符合业内通识（道德层面）

1. 规则

   ：不能用关键字：有特殊意义的字符，例：let，var，for。

   只能下划线，字母，$组成，且数字不能开头

   字母严格区分大小写！，如Age和age不同变量;

   2.规范

   起名要有意义

   遵守小驼峰写法

   第一个字母小写，后面每个单词字母大写。例：userName（用户）

# 变量词

Array(数组)

人：

 userName（用户）uname（姓名） age（年龄） gender（性别）

时间：

year（年），Month（月），Dater（日期）

数据：

number（ 数字 ）string（字符串） obj对象 （true） （对）   false（错）

max（最大值）min(最小值) 	undefined(未定义)	













## 1.数据类型-数字类型（Number）

数字可以有很多操作，比如*,除法/,加法+,减法-,所以算术运算符在一起.	数学运算符也叫<b>算术运算符</b>,主要包括加减乘除取余（求模)。

- 在 js  中所有的整数和浮点数 都是Number类型

- +：求和

- -：求差

- *:求积

- /:求商

- %:取模(取余数)

  - 开发中常常作为某个数字是否
  - 被整除判断.

  ### 1.3 javascript 算术运算符的优先级顺序

  通时使用多个运算符编写程序越优先被执行优先相同时以书从左向右执行。

  

  

## 2.string字符串型

- # 数据类型-字符串(string)

  

  字符串类型有个特点是用引号包裹

  ```html
  	""    ''  ``
  ```

  注意事项:

  1.无论单引号或是双引号必须成对使用

  2.单引号｜双引号可以互相嵌套，但不是自己嵌套自己（口诀外双，内单）

  3.必要时可以使用转移符\,输出引号或者双引号.

  <h1>字符串重点</h1>

​		➕号在字符串可以起到链接拼接

```js
        // 字符串拼接
        let age = prompt("输入年龄:")
        let lj = "老季"
        let hallo = "hallo"
        let puts = `你今年`
        document.write(hallo + lj + puts + age)
```

### 模版字符串

```javascript
  let age = prompt("输入你的年龄:");
        let lj = `大家好我是ikun,今年${age}岁，喜欢唱跳rap`;
        document.write(lj);
```

1. string 字符串型



1. boolean 布尔值

## 3.布尔值

​	true （对）   false（错）是布尔型字面量

null 和 nudefined区别：

- nudefined 表示没有赋值-放数据变成NaN
- null表示赋值了，但是内容为空

null开发中的使用场景：

官方解释：把null 作为未创建的对象

大白话：将来变量里面存放的是一个变量，但是对象还没创建好，可以先给个null

undefined 未定义型

null 空类型

NaN 代表一个计算错误.它是一个不正确的或者一个未定义的数字操作所得到的结果

<hr>


## 引用数据类型



- object 对象

# 检测数据类型

typeof 检查

```js
 let num = 10;
        console.log(typeof num);
        // 数字型
        let str = "ikun";
        console.log(typeof str);
```



# 数据-类型转换



在使用表单和 prompt获取过来的数据默认是字符串类型的，此时不能直接简单的进行加法的运算。

## 隐式转换

- a任何数据和字符串相加都是字符串



## 显示转换

parseInt 强行整数！

parseFloat 强行浮点！



```js
 <script>
        let numint = parseInt(prompt("整形"));
        console.log(typeof num1);
        let numfolat = parseFloat(prompt("浮点数："));
        console.log(typeof numfolat);
    </script>
```

小结 用户订单系统

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .box {
            width: 800px;
            height: 200px;
            margin: 0 auto;
            border: 1px solid #000;
        }
        
        table {
            margin: 0 auto;
            border-collapse: collapse;
        }
        
        table,
        tr,
        td {
            border: 1px solid rgb(12, 226, 34);
            font-weight: 100;
            animation: boder 2s infinite alternate;
        }
        
        @keyframes boder {
            0% {
                border-color: rgb(0, 0, 0);
            }
            100% {
                border-color: rgb(245, 243, 243);
            }
        }
    </style>
</head>

<body>

    <script>
        let sp = (prompt("输入购买商品名称:"));
        let yuan = parseInt(prompt("输入商品价格:"));
        let shuliang = parseInt(prompt("商品数量:"));
        let zong = yuan * shuliang;
        let dz = prompt("输入您的收获地址");
        document.write(`
        <table>
            <tr>
                <th>商品名称</th>
                <th>商品价格</th>
                <th>商品数量</th>
                <th>总价</th>
                <th>收获地址</th>
            </tr>
            <tr>
                <td>${sp}</td>
                <td>${yuan}元</td>
                <td>${shuliang}件</td>
                <td>${zong}元</td>
                <td>${dz}</td>
            </tr>
        </table>`)
    </script>
</body>

</html>
```



# 表达式

表达式也就是字面意思，用来表达一个结果

表达式和语句的区别

因为表达式可被求值，所以它可以在赋值语句的右侧。

而语句不一定有值，例：alert（）for和break等语句就不能被用于赋值。





# 分支语句

》程序三大流程控制语句	

## 顺序结构 字面意思从1开始顺序输出结构

## 分支结构 满足条件输出 不满足跳转分支

### if语句

- if语句有三种：单分支，双分支，多分支
- 单分支：

```js
if(条件){
  满足条件要执行的代码
}
```

​	》括号内的条件为true时，进入大括号里执行代码

​	》小括号内结果不是布尔值时，会发生隐士转换为布尔类型

​	》如果大括号只有一个语句，大括号可以省略，不建议这样书写✍️格式。

双分支if语法：

```js
if(条件){
	满足输出
}else{
  不满足输出
}
```

### 多分支

```javascript
if(条件1){
  输出1
}else if(条件2){
  输出2
}else if(条件3){
  输出3
}
```



# 案例-if配合运算符

求是闰年还是平年

```html
 <script>
        let year = prompt("输入年份");
        if (year % 4 === 0 && year % 100 !== 0 || year % 400 === 0) {
            alert(`${year}是闰年`);
        } else {
            alert(`${year}是平年`);
        }
    </script>
```

案例 成绩合格

    <script>
        //用户输入成绩
        let score = +prompt("请输入成绩");
        if (score >= 90) {
            alert("你很优秀哦～");
        } else if (score >= 70) {
            alert("成绩良好，加油");
        } else if (score >= 60) {
            alert("成绩及格，加油");
        } else if (score < 60) {
            alert("成绩不及格,请加油！");
        }
    </script>



	# 三元运算符



三元运算符的使用场景 ：三元是比if双分支更简洁的的写法

```html
条件？满足执行代码:不满足执行代码
 (3 > 5 ? "对" : "错")
3 < 5 ? alert(1) : alert(0)
```

一般用来取值

输入两个值做 比较：

```html
<script>
        let num = prompt("输入值");
        num = num < 10 ? 0 + num : num
        alert(num);
    </script>
```



# switch语句

```html
<script>
        switch (数据) {
            case 值1:
                代码1
                break
            case 值2:
                break
            case 值3:
                break
            case 值4:
                break
            default	：
            代码 n
            break
        }
  
</script>
  
  
   <script>
        let num = +prompt("输入值");
        switch (num) {
            case 1:
                alert("hallo");
                break
            case 2:
                alert("你好");
                break
            case 3:
                alert("傻逼");
                break
            case 4:
                alert("啦啦啦");
                break
            default:
                alert("没有符合条件");
                break
        }
    </script>
```

释义：

找到小括号的全等case值，输出相应代码

若没有全等===的执行default里面的代码

1. switch case语句一般用于等值判断，不断区间判断

2. switch case 一般要配合break关键字段使用 没有break会造成case穿透

   

   

   

   

   

   # 遍历循环

   ```js
    for (let i = 1; i <= arr.length; i++) {
      log(arr[i]);
    }
   ```

   获取数组长度

   .length

   

   for循环和while循环有什么区别呢:

   > 有明确的循环次数我们应该当使用for循环

   > 当补明确循环的次数的时候推荐使用while循环

   

   

   # 无限循环

   While(true)

   退出break

   ```js
        let i;
           while (true) {
               console.log(1);
           }
           for (;;) {
               //两个无限循环 退出循环使用break
           }
   ```

   

   ## 循环结束方法

   baerk 和 continue （结束本轮循环）

   baerk（直接结束循环） 



# 数组

基本使用

Length 数组长度

```js
     console.log(Arr.length);
```

在数组的数据编号叫下标或索引！

数组可以存粗任意类型的数据

数组的作用：单个变量可以存储多个数据。

```js
let Ayy =["ikun","kun","坤","ji"]
从0开始 ikun编号从0开始 
// 0，1，2，3


```

# 数据类型

基本数据类型：

1. Number 数字型

即我们数学中学习到的数字，可以是整数,小数，正数，负数。

##### 取数组最大或最小

```js
    <script>
        let arr = [2, 3, 5, 8];
        let max = arr[0];
        let min = arr[0];
        for (let i = 1; i < arr.length; i++) {
            if (max < arr[i]) {
                max = arr[i];
            }
            if (min < arr[i]) {
                console.log(`最小值为${min}`);
            }
        }
        console.log(`最大值为${max}`);
    </script>
```

## 操作数组

<ul>	数组本质就是数据集合，操作数据无非就是 增 删 改 查 语法</ul>

<h1>查</h1>：查询数组数据数组[下标]<br>或者我们访问数组数据

```js
script>
        let arr = [1, 4, 5, 7, 2, 9];
        for (let i = 0; i <= arr.length; i++) {
            console.log(arr[i]);
        }
    </script>
```



<h1>改</h1>	：	重新赋值 <br>数组[下标]=新值

```javascript
  <script>
        let arr = [];
        arr[1] = 1;
        arr[4] = 5;
        console.log(arr[1]);
        console.log(arr[4]);
    </script>
```



<h1>增</h1>:数据添加新的数据<br>arr.push(新增的内容)推 <br>arr.unshift(新增的内容)后	打印一下可以获取到最新的长度

```js
 <script>
        let arr = [1, 4, 5];
        arr.push("1");
        arr.unshift("hallo")
        arr.push("你好");
        console.log(arr);
        console.log(arr.push(1));	//最后一次可以获取最新的长度
    </script>
```



<h1>删</h1>:删除数组中的数据<br>arr.pop()删除最后的元素，一次一个<br>arr.shift()<br>arr.splice(操作的下标,删除的个数)

```js
  <script>
        let arr = [14, 23, 56, 78, 44, 55, 66];
        arr.pop() //        删除最后一个元素
        arr.shift() //      删除第一个元素
        console.log(arr);
        arr.splice(1, 5) //   arr.splice(从那个下标开始, 从那个下标结束)   
        console.log(arr);
    </script>
```

```text
	操作数组 -删除
	数组splice()方法 删除指定元素
	语法:
		arr.splice(start,deletecount)
		arr.splice(起始,删除几个元素)
```
# Flex 弹性盒模型

# 认识flex布局

box-shizing:border-box；



为什么要用flex布局？

答:在我们开发中利用弹性盒模型，可以快速开发减少设备之间的兼容问题，减少开发代码快速开发。

设置弹性盒子

  display: flex;

```css
    nav {
            display: flex;
            flex-direction: row;//水平行
      		 flex-direction: row-reverse;//水平反转
        }
```

![image-20230423154101879](/Users/a123/Library/Application Support/typora-user-images/image-20230423154101879.png)

```css
nav {
            display: flex;
            flex-direction: column;//列
  					 flex-direction: column-reverse;//反转列
        }
```

![image-20230423154301416](/Users/a123/Library/Application Support/typora-user-images/image-20230423154301416.png)



## flex-wrap 换行控制弹性盒子溢出问题

​	 折行

```css
 flex-wrap: wrap;//溢出换行
 flex-wrap: wrap-reverse;//反转换行
```

元素排列方式

```css
 flex-flow: column wrap-reverse;//设置列排列 溢出反转换行
```


