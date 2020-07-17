# Web 前端高级编程

## Web前端基础

### 常用标签

```html
<!-- html5 文档解析 -->
1.body 之间写网页内容
2.内容换行，浏览器解析的时候并不会换行，换行需要使用 <br> 进行换行
3.不管换行多少，空格多少，浏览器只会解析为一个空格
<!-- div 容器标签 -->
1.body 里面的标签都是一些盒子容器，可以装内容，甚至标签
2.一个div在网页中占一行，就类似文章中的段落
<!-- span 文本标签 -->
1.span 行内元素，通常用来定义 html 中文本的样式内容
<!-- img 图片标签 -->
img 是负责装图片的标签，src就是图片的路径（地址）
<!-- a 超链接标签 -->
a 标签是一个超链接，点击后可以跳转到其他页面，href就是跳转的地址
<!-- input 文本框 -->
input 文本框，可以接收用户输入的信息
<!-- button 按钮 -->
button 按钮，和用户交互，类似开关的作用
```

#### 文字修饰样式

```html
<!-- color 文字颜色 -->
color 文本颜色设置，可以设置颜色编码与颜色单词，#eee,#eeeeee,red
<!-- font-size 文字大小 -->
font-size 设置文字的大小，通常为 18px
<!-- font-family 字体 -->
font-family 设置文字的字体，字体可以设置为 黑体
<!-- font-weight 加粗 -->
font-weight 设置文字加粗，加粗 bold
<!-- text-decoration 下划线 -->
text-decoration 设置文字的下划线,underline 有下划线，none 无下划线
<!-- text-indent 段落缩进 -->
text-indent 对段落进行缩进，提高段落的美观程度， 100px
```

#### 其他常见样式

```html
<!-- brackground-color 背景色 -->
brackground-color 背景颜色，#eee,red
<!-- line-height 行高 -->
line-height 如果行高大于字体大小，那么文字就会居中
<!-- hover 伪类 -->
hover 设置在css中，鼠标移动到标签上就会触发伪类 a:hover 
<!-- text-align 文本位置对齐 -->
text-align 对标签内的文字进行位置控制，left 左对齐，center 居中，right 右对齐
<!-- widht 宽度，height 高度 -->
widht ，设置标签的宽度，height 设置标签的高度，
相对长度单位包括：em, ex, ch, rem, vw, vh, vmax, vmin
绝对长度单位包括：cm, mm, q, in, pt, pc, px
ch:数字“0”的宽度
em:相对于当前对象内文本的字体尺寸。如当前对行内文本的字体尺寸未被人为设置，则相对于浏览器的默认字体尺寸。
ex:相对长度单位。相对于字符“x”的高度。通常为字体高度的一半。如当前对行内文本的字体尺寸未被人为设置，则相对于浏览器的默认字体尺寸。
rem:相对于根元素(即html元素)font-size计算值的倍数
vw:相对于视口的宽度。视口被均分为100单位的vw
vh:相对于视口的高度。视口被均分为100单位的vh
vmax:相对于视口的宽度或高度中较大的那个。其中最大的那个被均分为100单位的vmax
vmin:相对于视口的宽度或高度中较大的那个。其中最大的那个被均分为100单位的vmax

cm:厘米     1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
mm:毫米    1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
q:1/4毫米   1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
in:英寸       1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
pt:点          1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
pc:派卡      1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
px:像素      1in = 2.54cm = 25.4 mm = 101.6q = 72pt = 6pc = 96px
```

| Pixels | EMs     | Percent | Points |
| ------ | ------- | ------- | ------ |
| 6px    | 0.375em | 37.5%   | 5pt    |
| 7px    | 0.438em | 43.8%   | 5pt    |
| 8px    | 0.5em   | 50%     | 6pt    |
| 9px    | 0.563em | 56.3%   | 7pt    |
| 10px   | 0.625em | 62.5%   | 8pt    |
| 11px   | 0.688em | 68.8%   | 8pt    |
| 12px   | 0.75em  | 75%     | 9pt    |
| 13px   | 0.813em | 81.3%   | 10pt   |
| 14px   | 0.875em | 87.5%   | 11pt   |
| 15px   | 0.938em | 93.8%   | 11pt   |
| 16px   | 1em     | 100%    | 12pt   |
| 17px   | 1.063em | 106.3%  | 13pt   |
| 18px   | 1.125em | 112.5%  | 14pt   |
| 19px   | 1.188em | 118.8%  | 14pt   |
| 20px   | 1.25em  | 125%    | 15pt   |
| 21px   | 1.313em | 131.3%  | 16pt   |
| 22px   | 1.375em | 137.5%  | 17pt   |
| 23px   | 1.438em | 143.8%  | 17pt   |
| 24px   | 1.5em   | 150%    | 18pt   |

#### 选择器

```css
/* 类选择器，改变相应类标签的样式 */
.div1{}
<div class="div1"></div>
/* 标签嵌套 */
/* 后代选择器 */
div strong{}
/* 子元素选择器 */
div>strong{}
/* 子元素优先级大于后代选择器 */
```

#### Google 案例

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Google案例</title>
	<style type="text/css">
		.blue {
			font-size: 100px;
			color: blue;
		}
		.red {
			font-size: 100px;
			color: red;
		}
		.orange {
			font-size: 100px;
			color: orange;
		}
		.green {
			font-size: 100px;
			color: green;
		}
	</style>
</head>
<body>
	<span class="blue">G</span>
	<span class="red">o</span>
	<span class="orange">o</span>
	<span class="blue">g</span>
	<span class="green">l</span>
	<span class="red">e</span>
</body>
</html>
```

### 盒子模型

- **Margin(外边距)** - 清除边框外的区域，外边距是透明的。
- **Border(边框)** - 围绕在内边距和内容外的边框。
- **Padding(内边距)** - 清除内容周围的区域，内边距是透明的。
- **Content(内容)** - 盒子的内容，显示文本和图像。

#### 边框

```css
/* 边框有上下左右边框，可分别设置，也可以同时设置 */
border: 上10px 右10px 下10px 左10px;
border: 上下10px 左右10px;
border: 上下左右10px;
border-top: 上边框
border-bottom: 下边框
border-left: 左边框
border-right: 右边框
/* 圆弧边框,一般为宽的一半即可*/
border-radius: 50px 
/* 取消轮廓线 */
outline:none
/* 盒子阴影 */
/* box-shadow:水平阴影 垂直阴影 模糊距离（虚实）  阴影尺寸（影子大小）  阴影颜色  内/外阴影 */
box-shadow:15px 15px 30px black;
```

#### 内边距

```css
/* 盒子内的距离，内边距 */
padding-top:;上内边距
padding-bottom:;下内边距
padding-left:;左内边距
padding-right:;右内边距
padding:; 所有内边距设置
```

#### 外边距

```css
/* 盒子对外的距离，外边距 */
margin-top:;上外边距
margin-bottom:;下外边距
margin-left:;左外边距
margin-right:;右外边距
margin:; 所有外内边距设置
/* 上下外边距，当两个标签存在上下外边距相邻关系时，会出现外边距重叠的现象，上下外边距会以最大的显示 */
/* 垂直外边距合并，父类标签和子类标签，当子类标签存在外边距，父标签没有外边距的时候，会合并为子父类外边距 */
/* 解决方法 */
/*嵌套关系 垂直外边距合并  解决方案 */
/*1. 可以为父元素定义上边框  transparent 透明*/
border-top: 1px solid transparent;
/*2. 可以给父级指定一个 上 padding值*/
padding-top: 1px;
/*3. 可以为父元素添加overflow:hidden。*/
overflow: hidden;
```

#### 盒子模型模式切换

```css
/* 盒子模型的模式 */
box-sizing:
/*分别有三种模式，不计算内外边距边框（默认），计算内外边距边框，继承父类内外边框*/
content-box, border-box, inherit
```

#### 网页设置，制作思路

1.从外到内

2.从上到下

3.从左到右

### 背景

```css
/* 背景图路径设置 */
background-image: url(images/bgc.png);
/* text decoration 文本装饰  none就是没有 */
text-decoration:none;
/* 变成行内块 */
display:inline-block
/* 行内元素 span a
    1.一行多个
    2.不可以设置高宽

    行内块 img
    1.一行多个
    2.可以设置高宽

    块级 div p h系列
    1.独占一行
    2.可以设置高宽 */

/* 背景图重复与不重复 */
/* 背景图不重复 */
 background-repeat: no-repeat;
/* 背景图横向重复 */
background-repeat: repeat-x;
/* 背景图纵向重复 */
background-repeat: repeat-y;

/* 背景图定位,定位背景图时需要取消掉背景图的重复 */
/* 背景图不重复 */
background-repeat: no-repeat;
/* 背景图定位，可以调整背景图从哪里开始显示 */
background-position: 10px 8px;

/* 背景图的显示比例 */
background-size: 100%;
```

### 透明与隐藏

```css
/* 不占位隐藏 */
display:none;
/* 占位隐藏 */
visibility:hidden;
/* 设置透明度 */
opacity:1;
/* 设置颜色的透明度 r就是红色 g就是绿色 b就是蓝色 这就是三原色  然后a就是 alpha 透明度 */
backgruond-color:rgba(30,77,179,0.1)
```

### 其他

```css
/* 选择器权重 */
/* css中用四位数字表示权重，权重的表达方式：0,0,0,0
标签选择器:0001
类选择器:0010
id选择器:0100
包含选择器的权重：包含的选择器权重之和
内联样式(行内样式)的权重：1000 */
/* !important权重是10000 */
div{
	background-color: blue!important;
}
/* 输入框属性 */
<input type=""></input>
button 	定义可点击按钮（多数情况下，用于通过 JavaScript 启动脚本）。
checkbox 	定义复选框。
file 	定义输入字段和 "浏览"按钮，供文件上传。
hidden 	定义隐藏的输入字段。
image 	定义图像形式的提交按钮。
password 	定义密码字段。该字段中的字符被掩码。
radio 	定义单选按钮。
reset 	定义重置按钮。重置按钮会清除表单中的所有数据。
submit 	定义提交按钮。提交按钮会把表单数据发送到服务器。
text 	定义单行的输入字段，用户可在其中输入文本。默认宽度为 20 个字符。
/* 标签多类 */
<div class="c1 c2 c3"></div>
```

#### 行元素与块元素

```html
<!-- ============================================ -->
<!-- =================  行属性  ================== -->
<!-- ============================================ -->
<!--
	<a>、<span>、<i>、<em>、<strong>、<label>、<q>、<var>、<cite>、<code>等
-->
<!--
    1.行属性标签它和其它标签处在同一行内
    2.行属性标签无法设置宽度，高度 行高 距顶部距离 距底部距离
    3.行属性标签的宽度是直接由内部的文字或者图片等内容撑开的
    4.行属性标签内部不能嵌套行属性标签（a链接内不能嵌套其他链接）
-->
<!-- ============================================ -->
<!-- =================  块属性  ================== -->
<!-- ============================================ -->
<!-- 
	<div>、<p>、<h1>…<h6>、<ol>、<ul>、<li>、<address>、<blockquote>、<form> 
-->
<!--
    1.每一个快属性标签都是从新的一行开始，而且之后的元素也都会从新的一行开始
    （因为每一个块属性标签都会直接占据一整行的内容，导致下面的内容也只能从新的一行开始）
    2.块属性标签都是可以设置宽度、高度，行高，距顶部距离，距底部距离
    3.块属性标签的宽度假如不做设置，会直接默认为父元素宽度的100%
    4.块属性标签是可以直接嵌套的
    5.p标签中不能嵌套div标签
-->
```

### 布局

#### Flex 弹性布局

http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html



## JavaScript 高级篇

### prototype 原型

``` js
function Fn(){
    
}
// protorype 就是原型,原型本质上也是对象
Fn.protorype.x=1
Fn.protorype.test = function(){
    console.log(this)
}

// new 一个函数生成的对象,可以访问中国函数原型 prototype

var o = new Fn()

o.x = 2
console.log(o.x)

// 对象原型
// 每一个对象都有一个__proto__，并且这个__proto__就是生成对象函数的prototype
console.log( o.__proto__ == Fn.prototype )

// 原型链
console.log( o.__proto__.__proto__ )

// 对象访问查找顺序
// 对象o优先访问自己的属性，找不到再去访问自己的__proto__，还找不到就去访问__proto__的属性，最后再去找__proto__.__proto__
console.log(o.x, o.__proto__.x);

// 原型对象 this 指向
// new一个函数生成的对象访问原型的方法，方法里面的this指向这个对象
o.test();
```

### 扩展内置对象方法

```js
// 使用 prototype 对对象创建新的方法
Date.prototype.format = function () {
    return this.getFullYear() + '-' + (this.getMonth() + 1)
}

// 创建对象
var d = new Date()

// 使用创建的方法
console.log(d.format());

Array.prototype.calc = function(){
    var s = 0
    for(var i = 0; i < this.length; i++){
        s += this[i]
    }
    return s
}

var arr = [1,2,3]
console.log( arr.calc() );
```

### 扩展日期方法

```js
Date.prototype.format = function (fmt) { //author: meizz   
    var o = {
        "M+": this.getMonth() + 1,                 //月份   
        "d+": this.getDate(),                    //日   
        "h+": this.getHours(),                   //小时   
        "m+": this.getMinutes(),                 //分   
        "s+": this.getSeconds(),                 //秒   
        "q+": Math.floor((this.getMonth() + 3) / 3), //季度   
        "S": this.getMilliseconds()             //毫秒   
    };
    if (/(y+)/.test(fmt))
        fmt = fmt.replace(RegExp.$1, (this.getFullYear() + "").substr(4 - RegExp.$1.length));
    for (var k in o)
        if (new RegExp("(" + k + ")").test(fmt))
            fmt = fmt.replace(RegExp.$1, (RegExp.$1.length == 1) ? (o[k]) : (("00" + o[k]).substr(("" + o[k]).length)));
    return fmt;
}

var d = new Date();

// yyyy代表年
// MM代表月
// dd代表日
// hh代表小时
// mm代表分钟
// ss代表秒

// 年月日
d.format('yyyy-MM-dd')

// 时分秒
d.format('yyyy-MM-dd hh:mm:ss')

// 年月日时分秒
d.format('yyyy-MM-dd hh:mm:ss')

// 年月日时分秒季
d.format('yyyy-MM-dd hh:mm:ss q')
```

### forEach 循环

```js
// forEach 迭代(遍历) 数组
var arr = [1, 2, 3];
var sum = 0;

for (var i = 0; i < arr.length; i++) {
    console.log('每个数组元素' + arr[i]);
    console.log('每个数组元素的索引号' + i);
    console.log('数组本身' + arr);
}
// 上下代码等价

// forEach也是循环，他会循环这个数组，把数组的每一个元素、下标分别传入里面的函数执行
arr.forEach(function (v, i, list) {
    console.log('每个数组元素' + v);
    console.log('每个数组元素的索引号' + i);
    console.log('数组本身' + list);
})
```

### filter 筛选数组

```js
// filter 筛选数组
var arr = [12, 66, 4, 88, 3, 7];
var newArr2 = []


// for(var i = 0; i < arr.length; i++){
//   if(arr[i] >= 20){
//     newArr2.push(arr[i])
//   }
// }
// console.log(newArr2)

// 上下代码等价

newArr2 = arr.filter(function(v){
    return v >= 20
})

console.log(newArr2);
```

### map 遍历数组

```js
var arr = [{
    name: 'iphone8',
    cateName:'苹果品牌',
    time: '2016-9'
}, {
    name: '荣耀8',
    cateName:'华为品牌',
    time: '2017-9'
}, {
    name: 'iphone7',
    cateName:'苹果品牌',
    time: '2015-9'
}]

// 转成['iphone8-苹果品牌','荣耀8-华为品牌','iphone7-苹果品牌']

// var arr2 = []

// for(var i = 0; i < arr.length; i++){
//   arr2.push(arr[i].name + '-' + arr[i].cateName)
// }

// console.log(arr2);

// 上下代码等价
var arr2 = arr.map(function(v){
    return v.name + '-' + v.cateName
})

console.log(arr2);
```

### JavaScript 正则使用

```js
// 正则表达式在js中的使用

// 1. 利用 RegExp对象来创建 正则表达式
var regexp = new RegExp(/^1[3-9]\d{9}$/)
console.log(regexp)

// 2. 手机号码正则表达式，一般通过百度  “正则 手机号码(身份证)” 寻找合适的正则
var rg = /^1[3-9]\d{9}$/
// 3.test 方法用来检测字符串是否符合正则表达式要求的规范
console.log(rg.test(13800000000))
console.log(rg.test('abc'))
```

### JavaScript 替换

```js
var str = 'abcdeabcdeabcde'

// 替换，下面代码的意思就是匹配a，g就是全局(匹配所有), 把所有的a替换成x
var str2 = str.replace(/a/g, 'x')

console.log(str);
console.log(str2)
```

### 默认 this 的指向

```js
// 函数的不同调用方式决定了this 的指向不同
// 1. 普通函数 this 指向window，浏览器上的对象和方法都是属于window的，但是一般可以省略写
function fn() {
    console.log('普通函数的this');
    console.log(this);
}
fn();

// 2. 对象的方法 this指向的是对象 o
var o = {
     sayHi: function() {
         console.log('对象方法的this:');
         console.log(this);
     }
}
o.sayHi();

// 3. 构造函数 this 指向 vm 这个实例对象 原型对象里面的this 指向的也是 vm这个实例对象
function Vue() {}
Vue.prototype.http = function() {
   console.log(this)
}
var vm = new Vue()
vm.x = 1
vm.http()

// 4. 绑定事件函数 this 指向的是函数的调用者 btn这个按钮对象
var btn = document.querySelector('button');
btn.onclick = function() {
     console.log('绑定点击事件函数的this:');
     console.log(this);
}
// 5. 定时器函数 this 指向的也是window
setTimeout(function() {
     console.log('定时器的this:');
     console.log(this);
}, 1000)
// 6. 立即执行函数 this还是指向window
(function() {
     console.log('立即执行函数的this');
     console.log(this);
})()
```

### 对象方法中的 this 指向

```js
// 2. 对象的方法 this指向的是对象 o
var o = {
    sayHi: function() {
        console.log('对象方法的this:');
        console.log(this);
    }
}
o.sayHi();

// 3. 构造函数 this 指向 vm 这个实例对象 原型对象里面的this 指向的也是 vm这个实例对象
function Vue() {}
Vue.prototype.http = function() {
   console.log(this)
}
var vm = new Vue()
vm.x = 1
vm.http()

// 4. 绑定事件函数 this 指向的是函数的调用者 btn这个按钮对象
var btn = document.querySelector('button');
btn.onclick = function() {
     console.log('绑定点击事件函数的this:');
     console.log(this);
}
// 5. 定时器函数 this 指向的也是window
setTimeout(function() {
     console.log('定时器的this:');
     console.log(this);
}, 1000)
// 6. 立即执行函数 this还是指向window
 (function() {
     console.log('立即执行函数的this');
     console.log(this);
})()
```

### new 函数里面的 this

```js
// // 3. 构造函数 this 指向 vm 这个实例对象 原型对象里面的this 指向的也是 vm这个实例对象
function Vue() {}
Vue.prototype.http = function() {
    console.log(this)
}
var vm = new Vue()
vm.x = 1
vm.http()

// 4. 绑定事件函数 this 指向的是函数的调用者 btn这个按钮对象
var btn = document.querySelector('button');
btn.onclick = function() {
     console.log('绑定点击事件函数的this:');
     console.log(this);
}
5. 定时器函数 this 指向的也是window
setTimeout(function() {
     console.log('定时器的this:');
     console.log(this);
}, 1000)
// 6. 立即执行函数 this还是指向window
(function() {
     console.log('立即执行函数的this');
     console.log(this);
})()
```

### dom 事件里面的 this

```js
// 4. 绑定事件函数 this 指向的是函数的调用者 btn这个按钮对象
var btn = document.querySelector('button');
btn.onclick = function() {
    console.log('绑定点击事件函数的this:');
    console.log(this);
}
```

### 改变函数内 this 指向(call,apply,bind)

```js
// 改变函数内this指向  js提供了三种方法  call()  apply()  bind()

// 1. call()
var o = {
    name: 'andy'
}

function fn(a, b) {
    console.log(this);
    console.log(a + b);
}
// fn(1, 2)

// call的第一个参数就是fn的this的指向，所以call可以动态改变这个函数的this指向
// call 第一个可以调用函数 第二个可以改变函数内的this 指向
fn.call(o, 1, 2)
// 上下等价
// 2. apply()  应用 运用的意思
fn.apply(o, [1, 2])

// 1. 也是调用函数 第二个可以改变函数内部的this指向
// 2. 但是他的参数必须是数组(伪数组)
// 3. apply 的主要应用 比如说我们可以利用 apply 借助于数学内置对象求数组最大值 
// Math.max();
// var arr = [1, 66, 3, 99, 4];
// var arr1 = ['red', 'pink'];
// // var max = Math.max.apply(null, arr);
// var max = Math.max.apply(Math, arr);
// var min = Math.min.apply(Math, arr);
// console.log(max, min);

// 3. bind()  绑定 捆绑的意思
// bind跟call和apply不一样，他不会马上执行这个函数fn，他会返回一个函数，这个函数的this和参数已经通过bind绑定好了，返回的这个函数可以直接执行不传参
var f = fn.bind(o, 1, 2);
f()
```

### JavaScript 闭包

```js
// 闭包（closure）就是一个函数可以读取另外一个函数的变量，那么这个函数就是闭包函数
function fn() {
    // 相当一个私有变量, 避免一些不小心修改到这个变量的情况
    // 这个局部变量会一直保留，不会被垃圾回收！！！！！！！！！！因此这种变量不能太多太大，不然容易内存泄露
    var num = 10;
    return function() {
        // 像这个y就会被回收的！！！
        var y = 1

        num++

        console.log(num);
    }
}
var f = fn();
f();
f();
f();
```

### 思考题

```js
// 思考题 1：

var name = "我是window对象的name"
var object = {
    name: "我是object对象的name",
    getNameFunc: function() {
        console.log(this)
        return function() {
            console.log(this)
            return this.name
        }
    }
};

console.log( object.getNameFunc()() );

// 思考题 2：

var name = "我是window对象的name";　　
var object = {　　　　
    name: "我是Object的name",
    getNameFunc: function() {
        var that = this
        return function() {
            return that.name;
        }
    }
}

console.log(object.getNameFunc()())

// 思考题 3：

var name = "我是window对象的name";
var object = {
    name: "我是Object的name",
    getNameFunc: function () {
        var that = this
        return function () {
            console.log(that);
            return that.name;
        }
    }
}

var f = object.getNameFunc

console.log(f()())
```

### JavaScript 递归

```js
// 递归函数 : 函数内部自己调用自己, 这个函数就是递归函数
var num = 1

function fn() {
    console.log('我要打印6句话');
    num++;
    if(num > 6){
        return
    }
    fn()
}

fn()

// 利用递归函数求1~n的阶乘 1 * 2 * 3 * 4 * ..n
// var sum = 1;
// var n = 6
// for (var i = 1; i <= n; i++) {
//   sum *= i
// }
// console.log(sum); 

// 上下等价

// function fn(n) {
//   if (n == 1) {
//     return 1;
//   }
//   return n * fn(n - 1);
// }
// 6 * fn(5)
// 6 * 5 * fn(4)
// 6 * 5 * 4 * fn(3)
// 6 * 5 * 4 * 3 * fn(2)
// 6 * 5 * 4 * 3 * 2 * fn(1)
// 6 * 5 * 4 * 3 * 2 * 1

// console.log(fn(6));

// 树结构
var data = [{
    id: 1,
    name: '家电',
    children: [{
        id: 11,
        name: '冰箱',
        children: [{
            id: 111,
            name: '海尔'
        }, {
            id: 112,
            name: '美的'
        },]
    }, {
        id: 12,
        name: '洗衣机',
        children: [{
            id: 121,
            name: '西门子'
        }, {
            id: 122,
            name: '小天鹅'
        },]
    }]
}, {
    id: 2,
    name: '服饰'
}];

// 遍历整棵树
// seek这个函数的功能就是打印数组的数据，如果这个数据有儿子就再次调用
function seek(data){
    for(var i = 0; i < data.length; i++){
        console.log(data[i].name)
        if(data[i].children){
            seek(data[i].children)
        }
    }
}

seek(data)
```

### JavaScript 数组拷贝

```js
// 浅拷贝类似 python = ,赋值地址
// 浅拷贝只是拷贝一层, 更深层次对象级别的只拷贝引用.
// 深拷贝拷贝多层, 每一级别的数据都会拷贝.
var obj = {
    id: 1,
    name: 'andy',
    msg: {
        age: 18
    }
}
var o = {}
o = obj


for (var k in obj) {
     // k 是属性名   obj[k] 属性值
     o[k] = obj[k];
}
console.log(o);
o.msg.age = 20;
console.log(obj);

console.log('--------------');
Object.assign(o, obj); //基本等价与for in的浅拷贝
console.log(o);
o.msg.age = 20;
console.log(obj);

// 深拷贝类似 python[:] ,赋值堆词值
// 深拷贝拷贝多层, 每一级别的数据都会拷贝.
var obj = {
    id: 1,
    name: 'andy',
    msg: {
        age: 18
    },
};
var o = {};

function deepcopy(t, o){
    for(var k in o){
        if(typeof o[k] == 'object'){
            t[k] = {}
            deepcopy(t[k], o[k])
        }else{
            t[k] = o[k]
        }
    }
}

deepcopy(o, obj)
console.log(o);
console.log(obj);
```

### JavaScript 判断类型终极方法

```js
// 判断类型的终极方法
console.log(Object.prototype.toString.call(1)  )
console.log(Object.prototype.toString.call("12") ) 
console.log(Object.prototype.toString.call([])  )
console.log(Object.prototype.toString.call({})  )
```

### let局部变量

```js
/*
    let关键字就是用来声明变量的
    使用let关键字声明的变量具有块级作用域
    在一个大括号中 使用let关键字声明的变量才具有块级作用域 var关键字是不具备这个特点的
    防止循环变量变成全局变量
    使用let关键字声明的变量没有变量提升
    使用let关键字声明的变量具有暂时性死区特性

*/

/* --------let关键字就是用来声明变量的-------- */
let a = 10;
console.log(a);

/* --------使用let关键字声明的变量具有块级作用域-------- */
if (true) {
let b = 20;
console.log(b)
if (true) {
	let c = 30;
}
	console.log(c);
}
console.log(b)

/* -------在一个大括号中 使用let关键字声明的变量才具有块级作用域 var关键字是不具备这个特点的--------- */

if (true) {
	let num = 100;
 	var abc = 200;
}
console.log(abc);
console.log(num)


/* -------防止循环变量变成全局变量--------- */
for (let i = 0; i < 2; i++) {}
console.log(i);


/*-----使用let关键字声明的变量没有变量提升------*/
console.log(a);
let a = 100;


/* -------使用let关键字声明的变量具有暂时性死区特性------- */
var num = 10
if (true) {
 	console.log(num);
	let num = 20;
}
```

### const 常量

```js
// 使用const关键字声明的常量具有块级作用域
if (true) {
	const a = 10;
 	if (true) {
 		const a = 20;
 		console.log(a);
 	}
 	console.log(a);
}
console.log(a);

// 使用const关键字声明的常量必须赋初始值
const PI = 3.14;

// 常量声明后值不可更改 
const PI = 3.14;
PI = 100;
const ary = [100, 200];
ary[0] = 123;
ary = [1, 2]
console.log(ary);
```

### 结构及方法汇总

```js
// 数组结构
// 数组解构允许我们按照一一对应的关系从数组中提取值 然后将值赋值给变量
let ary = [1, 2, 3]
let [a, b, c, d, e] = ary
console.log(a)
console.log(b)
console.log(c)
console.log(d)
console.log(e)

// 对象结构
// 对象解构允许我们使用变量的名字匹配对象的属性 匹配成功 将对象属性的值赋值给变量

let person = {name: 'lisi', age: 30, sex: '男'}
let { name, age, sex } = person
console.log(name)
console.log(age)
console.log(sex)

// 下面这种知道下就好
let {name: myName} = person
console.log(myName)
```

### 箭头函数
```js
// 箭头函数是用来简化函数定义语法的
const fn = function() {
   console.log(123)
}

const fn2 = () => {
	console.log(123)
}
fn2()

const fn3 = (a, b) => {
   return a + b;
}
fn3(2, 3)

// 在箭头函数中 如果函数体中只有一句代码 并且代码的执行结果就是函数的返回值 函数体大括号可以省略
const sum = (n1, n2) => n1 + n2
const result = sum(10, 20)
console.log(result)

// 在箭头函数中 如果形参只有一个 形参外侧的小括号也是可以省略的
const fn = v => {
 	alert(v)
}
fn(20)

// 箭头函数不绑定this 箭头函数没有自己的this关键字 如果在箭头函数中使用this this关键字看箭头函数外层函数的this是多少，就是多少，否则是window
let o = {
   x:1,
   fn:function(){
     console.log(this)
     let fn3 = () => {
       console.log(this)
     }
     let fn4 = function(){
       console.log(this)
     }
     fn3()
     fn4()
   },
   fn2:() => {
     console.log(this);
   }
}
o.fn()
o.fn2()
```

### 参数使用

```js
// 剩余参数
let arr = ['张三' , '李四', '王五']
console.log(...arr);

let ary1 = ['张三' , '李四', '王五']
let [s1, ...s2] = ary1
console.log(s1)
console.log(s2)


// 如果是多个参数传给一个...args，那么args就会变成一个数组
const sum = (...args) => {
	console.log(args);
};
sum(10, 20)
sum(10, 20, 30)

// 扩展运算符可以将数组拆分成以逗号分隔的参数序列
let ary = ["a", "b", "c"]
//...ary // "a", "b", "c"
console.log(...ary)
// 上下等价，把数组拆开成多个参数用逗号隔开
console.log("a", "b", "c")
```

### 合并数组

```js
// 扩展运算符应用于数组合并
let ary1 = [1, 2, 3]
let ary2 = [4, 5, 6]
// ...ary1 // 1, 2, 3
// ...ary1 // 4, 5, 6
let ary3 = [...ary1, ...ary2]
console.log(ary3)

// 合并数组的第二种方法
let ary1 = [1, 2, 3]
let ary2 = [4, 5, 6]

ary1.push(...ary2)
console.log(ary1)

// 利用扩展运算符将伪数组转换为真正的数组
var oDivs = document.querySelectorAll('div')
console.log(oDivs)
var ary = [...oDivs]
ary.push('a');
console.log(ary);
```

### repeat 重复字符串

```js
// repeat就是字符串重复，比如下面就是重复5次
console.log("y".repeat(5))
```

### find 查找数组需要内容

```js
var ary = [{
    id: 1,
    name: '张三'
}, {
    id: 2,
    name: '李四'
}]
// 根据find传进去的函数的返回值条件找元素，只能循环数组第一层，不能找树结构
let target = ary.find(function(item){
   return item.id == 2
})
// 上下等价
let target = ary.find(item => item.id == 2)
console.log(target)
```

### findindex 查找数组内容下标位置

```js
let ary = [10, 20, 50]
// 跟find一样用法，只不过找的是下标
let index = ary.findIndex(item => item > 15)
console.log(index)
```

### includes 匹配字符串

```js
let ary = ["a", "b", "c"]
// includes就是找数组或者字符串里面是否包含这个参数(比如下面的a字符串)，包含就返回true，否则就false
let result = ary.includes('a')
console.log(result)
result = ary.includes('e')
console.log(result)

var str = 'iphoneX'
console.log( str.includes('iphone') );
```

### 模板字符串,和拼接字符串类似

```js
let name = '小明'
let sayHello = 'Hello, 我的名字叫' + name

// 模板字符串，换行不报错！并且可在字符串里面插入变量，通过${变量名}，再也不需要 + 号了

let sayHello1 = `Hello, 我的名字叫${name}`
console.log(sayHello1);

let result = {
    name: "zhangsan",
    age: 20
};

let html = `
    <div>
    <span>${result.name}</span>
    <span>${result.age}</span>
    </div>
`;
console.log(html);
```

### 判断字符串(startsWith,endsWith)

```js
let str = 'Hello ECMAScript 2015'

// 判断字符串str是否以'Hello'为开头
let r1 = str.startsWith('Hello')
console.log(r1);
// 判断是否以'2016'为结束
let r2 = str.endsWith('2016')
console.log(r2)
```

### 将伪数组转换为真数组

```js
// 伪数组
var arrayLike = {
    "0": "张三",
    "1": "李四",
    "2": "王五",
    "length": 3
}

// 就是可以把类似数组的元素转成数组
var ary = Array.from(arrayLike)
console.log(ary)

var arrayLike = {
    "0": "1",
    "1": "2",
    "length": 2
}

var ary = Array.from(arrayLike, item => item * 2)
console.log(ary)
```

JavaScript set 集合 用法

```js
const s1 = new Set()
console.log(s1.size)

const s2 = new Set(["a", "b"])
console.log(s2.size)

// Set就是数学里面的集合，集合有个特点，就是不重复, 利用这个特点就可以数组去重！！！
const s3 = new Set(["a","a","b","b"])
console.log(s3.size)
const ary = [...s3]
console.log(ary)

const s4 = new Set()
// 向set结构中添加值 使用add方法
s4.add('a').add('b')
console.log(s4.size)

// 从set结构中删除值 用到的方法是delete
const r1 = s4.delete('c')
console.log(s4.size)
console.log(r1)

// 判断某一个值是否是set数据结构中的成员 使用has
const r2 = s4.has('d')
console.log(r2)

// 清空set数据结构中的值 使用clear方法
s4.clear()
console.log(s4.size)

// 遍历set数据结构 从中取值
const s5 = new Set(['a', 'b', 'c'])
s5.forEach(value => {
    console.log(value)
})

const s6 = new Set(['a', 'b', 'c', 'a', 'b'])
const arr = Array.from(s6)
console.log(arr)
```

### 对象的简介使用

```js
// 键值同名，可省略写成一个
let name = '小明'

let obj = {
    name:name
}

//上下等效

let obj = {
    name
}

console.log(obj)

// 简写函数
let obj = {
  name:'小王',
  xueli:'本科',
  haha: function() {
    console.log('我在笑！')
  }
}

// 上下等价，下面是函数在对象里面可以简写

let obj2 = {
  name:'小王',
  xueli:'本科',
  haha(){
    console.log('我在笑！')
  }
}
```

### JavaScript 类

```js
// 对象
let zs1 = {
    name: '宇智波佐助',
    attack() {
        console.log('我砍！');
    }
}

// 类
class Fighter {
    type = '战士'

    // 构造函数，可以初始化一些信息
    constructor(name) {
        this.name = name
    }

	// 实例方法
    attack() {
        console.log('我砍！');
    }
}

// 类的继承
class Hero {
    constructor(name){
        this.name = name
    }
    say(str){
        console.log( str );
    }
}


// extends就是继承
class Fighter extends Hero {
    type = '战士'
    constructor(name){
        // super就是调用父亲的构造函数
        super(name)
    }
    attack(){
        console.log('拿刀砍你');
    }
}
```

### 跨域请求

页面的协议、端口号、主机地址(域名或者IP)如果和 你ajax请求的服务器的 协议、端口号、主机地址(域名或者IP)，有一个不一样，就是跨域请求

#### script 与跨域

```html
<!-- 1.将非同源服务器端的请求地址写在script标签的src属性中 -->
<!-- script标签是支持跨域的，只不过只能get请求 -->
<script src="http://localhost:3000/data"></script>
```

#### 使用接口接受跨域请求

```html
<script>
    function cb(data) {
        console.log('客户端的cb函数被调用了')
        console.log(data);
    }
</script>
<!-- 后端的jsonp接口返回一个字符串  "cb('后端的数据')"  长得像函数，
浏览器会执行这个函数，这样就可以通过js拿到数据填写到页面上 -->
<!-- 请求中后端调用了前段的函数,证明前后端已经交互 -->
<script src="http://localhost:3000/jsonp"></script>
```

```js
// 跨域jsonp请求
app.get('/jsonp', function (req, res) {
  res.send('cb("我是后端的数据")');
});
```

#### 标签加接口使用跨域请求

```html
<button id="btn">点我发送请求</button>
<script>
    function cb (data) {
        console.log('客户端的cb函数被调用了')
        console.log(data);
    }
</script>
<script type="text/javascript">
    // 获取按钮
    var btn = document.getElementById('btn');
    // 为按钮添加点击事件
    btn.onclick = function () {
        // 创建script标签
        var script = document.createElement('script');
        // 设置src属性
        script.src = 'http://localhost:3000/jsonp';
        // 将script标签追加到页面中
        document.body.appendChild(script);
        // 为script标签添加onload事件
        script.onload = function () {
            // 将body中的script标签删除掉
            document.body.removeChild(script);
        }
    }
</script>
```

```js
// 跨域jsonp请求
app.get('/jsonp', function (req, res) {
  res.send('cb("我是后端的数据")');
});
```

## GIT多人开发版本管理工具

[run serve 下载GIT版本管理工具](https://git-scm.com/)

免费GIT仓库

[码云(国内)](https://gitee.com)

[github(国外)](https://github.com/)

### 简易的命令行入门教程:

```shell
# Git 全局设置:
git config --global user.name "NingWilliam"
git config --global user.email "741554524@qq.com"

# 创建 git 仓库:
mkdir item_1
cd item_1
git init
touch README.md
git add README.md
git commit -m "first commit"
git remote add origin https://gitee.com/ming_xinChen/item_1.git
git push -u origin master
```

### 常见命令

```shell
// 下载项目
git clone 项目地址 (一般上班项目地址可以跟项目经理或者其他相关工作人员要)

// 提交代码三部曲
//提交到本地暂存区
git add .

//提交的本地仓库
git commit -m '你这次提交代码的说明'

// 提交到服务器
git push 最终提交

// 更新其他合作开发者的代码
git pull

// 查看文件提交状态(比如你某些文件没提交，他就会给你提示，如果没有提示说明都提交了)
git status -s
// 把提交到暂存区的代码删除，意思就是撤销 git add
git reset head
// 查看版本号，最好用git自带的bash命令行，就不会有bug
git log

// 本地仓库回退上一个版本，一个^代表上一个，两个^代表上两个，也可以直接指定版本号
// 相当于撤销 git commit
// 如果已经git push过了，就会产生冲突，建议使用revert回退！
git reset --hard HEAD^

// 回退上一个版本
git revert HEAD
```

### 过滤文件

创建一个叫 .gitignore 的文件，可以过滤掉不想提交的文件，比如node_module太大了无需提交

**支持格式**

1.直接输入文件夹或者文件名

2.*代表匹配所有

**多人合作分支版本命令**

```shell
// 查看版本
git branch
// 创建分支版本
git branch 版本名
// 删除本地分支版本
git branch -d 版本名
// 切换分支版本
git checkout 版本名
// 版本合并
git merge 版本名
```

## node.js

### node.js的使用

```bash
# 使用node 运行js文件
node js文件名
```

### 创建 http 服务器

```js
// const 定义一个常量，无法修改
// require 用来导入其他模块 module
// http 是服务器模块
const http = require('http');
// 内置方法有 createServer 创建服务
// req: 请求信息， res: 响应信息
http.createServer((req, res) => {
    // 请求方的地址
    console.log(req.url)
    // 服务器返回信息给请求方，（使用浏览器访问该端口的用户）
    res.end('这里是返回的信息')
    // listen 设置端口号的信息，可以使用 localhost:3000 对该服务器进行访问（首先需要运行该js）
}).listen(3000);
```

### 读取文件

```js
// 使用文件流系统，导入 fs 模块（文件系统）
const fs = require('fs');
// 使用内置 readFileSync 方法读取文件信息
// 格式为: object.readFileSync('文件路径','文件编码格式')
let str = fs.readFileSync('./1.txt', 'utf-8');
// 打印读取的文件信息
console.log(str);
```

### 写入文件

```js
// 使用文件流信息，导入 fs 模块（文件系统）
const fs = require('fs');
// 使用内置的 writeFileSync 方法写入文件
// 格式为: object.writeFileSync('文件路径','写入文件内容','写入文件编码格式')
let err = fs.writeFileSync('./2.txt', 'hijk', 'utf-8');
// 打印信息，成功返回 undefined 信息，失败返回失败信息
console.log(err);
```

### 向返回请求中传入网页

```js
// 导入模块
const http = require('http');
const fs = require('fs');
// 创建服务器
http.createServer((req, res) => {
    // 读取 html 文件信息
 	let html = fs.readFileSync('./index.html', 'utf-8');
    // 返回网页信息
 	res.end(html);
}).listen(3000);
```

### 根据地址返回网页

```js
// 导入模块
const http = require('http');
const fs = require('fs');

// 创建服务器
http.createServer((req, res) => {
    // 如果访问的地址为 / ，返回 ./index.html 文件
    // 如果访问的地址为 /list ， 返回 ./list.html 文件
 	if(req.url == '/'){
  		res.end(fs.readFileSync('./index.html', 'utf-8'));
 	}else if(req.url == '/list'){
        res.end(fs.readFileSync('./list.html', 'utf-8'));
    }
}).listen(3000);

```

## Ajax

### server.js 所有的接口

```js
const express = require('express');
const app = express();
const cookieParser = require('cookie-parser');
const bodyParser = require('body-parser');
const cors = require('cors');
const path = require('path');
const fs = require('fs');
const multer = require('multer')
const upload = multer({
  storage: multer.diskStorage({
    destination: function (req, file, cb) {
      cb(null, 'public/upload/')
    },
    filename: function (req, file, cb) {
      cb(null, Date.now() + file.mimetype.replace('image/', '.'))
    }
  })
})

// 允许浏览器跨域
app.use(cors());

// 只允许http://localhost:9000跨域
// app.use(cors({
//   origin: 'http://localhost:9000'
// }));
// cookie处理插件
app.use(cookieParser());
// 设置静态文件的文件夹
app.use(express.static('public'));

// 解析 application/json
app.use(bodyParser.json());
// 解析 application/x-www-form-urlencoded
app.use(bodyParser.urlencoded());

// 设置模板的路径
app.set('views', path.join(__dirname, 'views'));
// 设置使用哪个模板引擎，需要安装相关的模板引擎比如ejs
app.set('view engine', 'ejs');

// 普通get请求
app.get('/data', function (req, res) {
  res.send('这是后端返回给你的数据');
});



// 后端响应头设置json，返回json
app.get('/json', function (req, res) {
  res.json({
    name: '小明',
    age: 20
  });
});


// get请求传参
app.get('/query', function (req, res) {
  const { username, age } = req.query;
  res.send(`我叫${username}, 今年${age}岁！`)
});

// post请求
app.post('/form', function (req, res) {
  const { username, age } = req.body;
  res.send(`我叫${username}, 今年${age}岁！`)
});

// post上传文件
app.post('/upload', upload.single('img'), function (req, res) {
  res.json(req.file);
});


app.get('/data1', function (req, res) {
  setTimeout(() => {
    res.send('这是后端返回给你的数据1');
  }, 700);
});
app.get('/data2', function (req, res) {
  setTimeout(() => {
    res.send('这是后端返回给你的数据2');
  }, 1000);
});
app.get('/data3', function (req, res) {
  setTimeout(() => {
    res.send('这是后端返回给你的数据3');
  }, 500);
});


// restful风格的其他方法
app.put('/put', function (req, res) {
  res.send(`我是put请求，一般是修改资源`)
});

app.delete('/delete', function (req, res) {
  res.send(`我是delete请求，一般是删除资源`)
});


// 状态码系列开始 -------------------------
app.get('/200', function (req, res) {
  res.statusCode = 200;
  res.send('200状态码代表成功');
})

app.post('/201', function (req, res) {
  res.statusCode = 201;
  res.send('201状态码代表创建了新资源, 比如新增商品');
})

app.get('/301', function (req, res) {
  res.statusCode = 301;
  res.redirect('/301_2');
})

app.get('/301_2', function (req, res) {
  res.statusCode = 301;
  res.send('301代表永久重定向到某个新地址, 请注意看响应头的Location字段');
})

app.get('/302', function (req, res) {
  res.statusCode = 302;
  res.redirect('/302_2');
})

app.get('/302_2', function (req, res) {
  res.statusCode = 302;
  res.send('302代表临时重定向到某个新地址, 请注意看响应头的Location字段');
})

// 访问静态图片可看到304, http协议缓存, 响应头查看文件类型

app.get('/400', function (req, res) {
  if (Number(req.query.id) > 0) {
    res.send(`请求参数正确, ID为${req.query.id}, 大于0`);
  } else {
    res.statusCode = 400;
    res.send(`400代表请求参数错误, ID为${req.query.id}, 不大于0`)
  }
})

app.get('/401', function (req, res) {
  res.statusCode = 401
  res.send('401代表需要登录验证')
})

app.get('/403', function (req, res) {
  res.statusCode = 403
  res.send('403代表因未知原因拒绝你访问')
})

app.get('/404', function (req, res) {
  res.statusCode = 404;
  res.send(`404代表找不到资源`)
})

app.get('/500', function (req, res) {
  throw new Error('500代表服务端未知错误')
})
// 状态码系列结束 -------------------------


// 跨域jsonp请求
app.get('/jsonp', function (req, res) {
  res.send('cb("我是后端的数据")');
});


app.listen(3000, () => {
  console.log('3000端口服务开启');
})
```

### 传送请求，渲染文件

```html
<body>
  <div class="text"></div>
  <button>发送请求</button>
  <script type="text/javascript">
  	document.querySelector('button').addEventListener('click', function () {
        // 1.创建ajax对象
        var xhr = new XMLHttpRequest()
        // 2.告诉Ajax对象要向哪发送请求，以什么方式发送请求
        // 1)请求方式 2)请求地址
        xhr.open('get', 'http://localhost:3000/data')
        // 3.发送请求
        xhr.send()
        // 4.获取服务器端响应到客户端的数据
        xhr.onload = function () {
            // console.log(xhr.responseText);
            document.querySelector('.text').innerHTML = xhr.responseText
        }
    });
  </script>
</body>
</html>
```

### 解析json文件，并发送json数据

``` js
// 1.创建ajax对象
var xhr = new XMLHttpRequest();
// 2.告诉Ajax对象要向哪发送请求，以什么方式发送请求
// 1)请求方式 2)请求地址
xhr.open('get', 'http://localhost:3000/json');
// 3.发送请求
xhr.send();
// 4.获取服务器端响应到客户端的数据
xhr.onload = function (){
    // console.log(xhr.responseText)
    // 将JSON字符串转换为JSON对象
    var responseText = JSON.parse(xhr.responseText);
    // // // // 测试：在控制台输出处理结果
    console.log(responseText)
    // // // // 将数据和html字符串进行拼接
    var str = '<h2>'+ responseText.name +'</h2>';
    // // // // 将拼接的结果追加到页面中
    document.body.innerHTML = str;
}
```

### Promise 处理队列

Promise 是 es6 的新语法

```js
// new Promise会生成一个 Promise对象，Promise里面需要传一个函数，这个函数有两个参数
// Promise对象会有状态，默认是Pending状态
let p = new Promise((resolve, reject) => {
	// 当你执行 resolve 函数并传参，那么 Promise 状态会变成 resolved，并且Promise的值变成你传的参数
    // resolve() 正确信息传递
	// resolve(参数)
	// 当你执行 reject 函数并传参，那么Promise状态会变成 rejected，并且 Promise 的值变成你传的参数,并且会报错   
    // reject() 错误信息传递
    // reject(参数)
})
console.log(p);
```

Promise 封装 ajax

```js
/*
   基于Promise发送Ajax请求
*/
function queryData(url) {
    var p = new Promise(function (resolve, reject) {
        var xhr = new XMLHttpRequest();
        xhr.onreadystatechange = function () {
            if (xhr.readyState != 4) return;
            // xhr.readyState 是 Ajax 的状态值,这里的意思是当 Ajax 和 网页状态值一样的时候,进行下面的代码
            if (xhr.readyState == 4 && xhr.status == 200) {
                // 处理正常的情况
                // 只要执行了resolve，Promise对象就成功了，会变成resolved状态
                resolve(xhr.responseText);
            } else {
                // 处理异常情况
                // 只要执行了reject，Promise对象就失败了，会变成reject状态
                reject('错误');
            }
        };
        xhr.open('get', url);
        xhr.send();
    });
    return p;
}

// queryData('http://localhost:3000/data')
// .then(res => {
//   console.log(res);
// })

// queryData('http://localhost:3000/data')
//   .then(function (data) {
//     console.log('resolve执行了就会到这里来');
//     console.log(data);
//   });

// 如果Promise执行了resolve，那么resolve的传参会到then的第1个函数的参数里面
// 如果Promise执行了reject，那么reject的传参会到then的第2个函数的参数里面
queryData('http://localhost:3000/400').then(function (data) {
    console.log('resolve执行了就会到这里来');
    console.log(data);
}, function (err) {
    console.log('reject执行了就会到这里来');
    console.log(err)
});
```

Ajax 状态值

```shell
0：请求未初始化，还没有调用 open()。

1：请求已经建立，但是还没有发送，还没有调用 send()。

2：请求已发送，正在处理中（通常现在可以从响应中获取内容头）。

3：请求在处理中；通常响应中已有部分数据可用了，没有全部完成。

4：响应已完成；您可以获取并使用服务器的响应了。
```

### catch 最终执行

```js
/*
      Promise常用API-实例方法
    */
    // console.dir(Promise);
    function foo() {
      return new Promise(function(resolve, reject){
        setTimeout(function(){
          // resolve(123);
          reject('error');
        }, 100);
      })
    }
    foo()
      .then(function(data){
        console.log(data)
      })
      .catch(function(err){
        console.log('只要你执行了reject，最终都会到catch')
      })
```

## axios

```js
// axios是一个调接口的库，必须要熟练掌握，以下是get请求
axios.get('http://localhost:3000/json').then(res => {
    console.log(res.data)
})
```

### get请求传参

```js
/*
  axios请求参数传递
*/
// axios get请求传参
// 请求地址后面跟?，?后面就是参数=值，从第二个参数开始就是用&，&后面也是参数=值
axios.get('http://localhost:3000/400?id=123&n=9&u=8').then(res => {
    console.log(res.data);
});
// axios.get('http://localhost:3000/400?id=123&name=ken').then(res => {
//   console.log(res.data);
// });
```

### axios 全局配置

```js
/*
   axios 响应结果与全局配置
*/

// 配置请求的基准URL地址，就是每次调接口会把地址前面加上baseURL
axios.defaults.baseURL = 'http://localhost:3000'

// 超时中断接口时间，如果调接口超过这个毫秒数，会自动中断
// 有时候服务器处理接口卡住了，这个时候前端不可能一直等待，所以可以设置超时时间
// 5000就是5秒
axios.defaults.timeout = 5000

axios.get('/json').then(res => {
    console.log(res.data);
})
```

### post请求传参

```js
/*
   axios 响应结果与全局配置
*/

// 配置请求的基准URL地址，就是每次调接口会把地址前面加上baseURL
axios.defaults.baseURL = 'http://localhost:3000'

// 配置请求头信息
// java的后端一般设置x-www-form-urlencoded表单格式
// 使用java后端的 Post 请求的时候需要加上以下配置
// axios.defaults.headers['content-type'] = 'application/x-www-form-urlencoded'

// post与get的区别
// post传参可以传很大！！甚至文件，get传参只能传很小，无法文件
// post传参是在请求实体里面，get传参是地址后面跟参数


axios.post('/form', {
    username:'小明',
    age:22,
}).then(res => {
    console.log(res.data);
})
```

### 上传文件

```js
/*
  axios 响应结果与全局配置
*/

// 配置请求的基准URL地址，就是每次调接口会把地址前面加上baseURL
axios.defaults.baseURL = 'http://localhost:3000'

// 超时中断接口时间，如果调接口超过这个毫秒数，会自动中断
// 有时候服务器处理接口卡住了，这个时候前端不可能一直等待，所以可以设置超时时间
// axios.defaults.timeout = 5000

// 配置请求头信息
// axios.defaults.headers['content-type'] = 'application/x-www-form-urlencoded'

// 查找button标签,添加监听事件
document.querySelector('button').addEventListener('click', function () {


    // 如果是上传文件，得传FormData类型
    let formData = new FormData()

    formData.append('img', document.querySelector('input').files[0])

    axios.post('/upload', formData).then(res => {
        console.log(res.data);
    })

})
```

### axios 拦截器

```js
/*
   axios拦截器
*/

axios.defaults.baseURL = 'http://localhost:3000'

//  请求拦截器
// axios.interceptors.request.use(req => {
//   // java的后端一般设置x-www-form-urlencoded表单格式
//   if(req.method.toLowerCase() == 'post'){
//     req.headers['content-type'] = 'application/x-www-form-urlencoded'
//   }
//   return req
// })

// response响应拦截器
axios.interceptors.response.use(res => {
    // 每次调接口后端返回后，都会先走拦截器，再走我自己的then回调
    // console.log(res)
    // 提前把res的data点出来返回给我的then成功回调函数，这样就不用每次都点data出来了
    // 返回数据给网页
    return res.data
}, function(err){
    console.log(err)
})

axios.post('/form', {
    username:'adasd',
    age:22,
}).then(res => {
    console.log(res);
})
```

### axios 异步请求

```js
/*
   axios拦截器
*/

axios.defaults.baseURL = 'http://localhost:3000'

// 下面 then 中 console.log 会比网页中的 console.log 加载时间慢
// then 是等网页加载和 ajax 加载完成后进行后打印,网页中会直接打印
axios.post('/form', {
    username:'adasd',
    age:22,
}).then(res => {
    console.log(res);
})

console.log(11111);
```

### async / await 处理异步操作

```js
/*
   async/await 处理异步操作：
   async函数返回一个Promise实例对象
   await后面可以直接跟一个 Promise实例对象
*/
axios.defaults.baseURL = 'http://localhost:3000';

// async await 是2017年才出来的语法 

// 在函数前面加async关键字，这个函数就变成了 async 函数，async 函数返回的是 Promise，
// 并且 await 必须在 async 函数里面才合法
async function x() {
    // await 后面跟的是 Promise 对象
    let res = await axios.get('/data')
    console.log(res.data)
    let res2 = await axios.get('/data2')
    console.log(res2.data)
    let res3 = await axios.get('/data3')
    console.log(res3.data)
}

let y = x()
console.log(y)
```

### axios 语义化接口,(增删改查)

```js
/*
   axios 响应结果与全局配置
*/

// 语义化接口
// 获取 get
// 新增 post
// 修改 put
// 删除 delete


// 配置请求的基准URL地址，就是每次调接口会把地址前面加上baseURL
axios.defaults.baseURL = 'http://localhost:3000'

// 需要配置接口信息,不然回调提示 404

// 修改
axios.put('请求地址', {
    username:'adasd',
    age:22,
})

// 删除
axios.delete('请求地址')
```

### 网页状态码

```shell
200 响应成功
201 新增成功
301 永久重定向
302 临时重定向
304 返回缓存
400 请求参数错误
401 没有登录
403 没有权限
404 找不到资源
500 服务端异常
```

## web框架 - express

###  npm 常见命令

```bash
# 初始化npm项目
npm init -y

# 安装插件
npm install 插件名
# 或
npm i 插件名

# 设置镜像源为淘宝源
npm config set registry https://registry.npm.taobao.org

# supervisor可以监听文件修改，修改文件后不用重启node服务 -g是全局安装，不是单单安装进项目
npm i supervisor -g
```

### 安装 express 框架

```shell
npm i express
```

### 接口

```js
// 根据不同的接口，返回不同的信息
app.get('/', (req, res) => {
 res.send('我是首页');
});

app.get('/list', (req, res) => {
 res.send('我是列表');
});
```

### 返回静态资源

```js
// path: 用来处理地址信息，内有方法 path.join ，用来合并多个地址
const path = require('path');

// static 是静态文件夹，设置静态文件，使静态文件夹里面的文件可以直接访问，因为express会根据路径自动帮你读取这个文件
app.use(express.static(path.join(__dirname, 'public')));
```

### 返回动态网页

```shell
// 安装 ejs 模块
npm i ejs
```

### 使用方法

```js
app.set('views', path.resolve(__dirname, 'view'));
app.set('view engine', 'ejs');
```

```js
app.get('/', (req, res) => {
 	res.render('index', {title:'网页'});
});
app.get('/list', (req, res) => {
	res.render('list', {list:[{name:'iphone6'},{name:'iphone7'},{name:'iphoneX'}]});
});
```

## Vue 前端框架

### 使用方法

```html
<!-- 链接引用,使用最新的版本 -->
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
<!-- 链接引用,使用对应的版本 -->
<script scr="https://cdn.jsdelivr.net/npm/vue@2.6.11"></script>
<!-- 使用原生 ES Modules -->
<script type="module">
	import Vue from 'https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.esm.browser.js'
</script>
```

### NPM 安装

```shell
#最新稳定版本
npm install vue
```

Vue 安装目录,方便本地应用 Vue.js

|                          | UMD                | CommonJS              | ES Module(基于构建工具使用) | ES Module(直接用于浏览器) |
| ------------------------ | ------------------ | :-------------------- | --------------------------- | ------------------------- |
| 完整版                   | vue.js             | vue.commod.js         | vue.esm.js                  | vue.esm.browser.js        |
| 只包含运行时版           | vue.runtime.js     | vue.runtime.commom.js | vue.runtime.esm.js          | -                         |
| 完整版(生产环境)         | vue.min.js         | -                     | -                           | vue.esm.browser.min.js    |
| 只包含运行时版(生产环境) | vue.runtime.min.js | -                     | -                           | -                         |

#### 术语

- 完整版:同时包含编译器和运行时的版本
- 编译器:用来将模板字符串编译成为JavaScript渲染函数的代码
- 运行时:用来创建Vue实例、渲染并处理虚拟 DOM 等的代码 基本上就是出去编辑器的其他一切
- UMD:UMD版本可以通过`<script>`标签直接用在浏览器中.jsDelivr CDN 的https://cdn.jsdelivr.net/npm/vue 默认文件就是运行时 + 编辑器的 UMD 版本(`vue.js`)
- CommonJS:CommonJs版本用来配合老的打包工具比如Browserify 或 webpack 1. 这些打包工具的默认文件(`pkg.main`)是只包含运行时的CommonJS版本(`vue.runtime.common.js`).
- ES Module:从2.6开始Vue会提供两个ES Modules(ESM)构建文件:
  - 为打包工具提供ESM:为诸如webpack 2 或Rollup 提供的现代打包工具.ESM格式被设计为可以被静态分析,所以打包工具可以利用这一点来进行"tree-shaking"并将用不到的代码排除最终的包.为这些打包工具提供的默认文件(`pkg.module`)是只有运行时的ES Module 构建(`vue.runtime.esm.js`).
  - 为浏览器提供的 ESM (2.6+):用于在现代浏览器中通过 `<script type="module">` 直接导入.

## Vue 前段框架，项目篇

### 项目1.商品管理系统

#### 项目介绍

- 用户分页界面
  - 新增用户，编辑用户，修改用户权限，删除用户
- 商品分页界面
  - 新增商品，编辑商品，删除商品
- 品牌列表界面
  - 新增品牌，编辑品牌，删除品牌
- 分类列表界面
  - 新增分类，编辑分类，删除分类
- 角色列表界面
  - 修改角色权限，新建角色，删除角色
- 销售数据界面
  - 使用 v-charts 对数据进行销售绘图

#### 项目亮点

可批量对用户进行修改权限，不同的权限能够使用不同的功能

#### 项目代码及步骤解析

项目的开始登陆界面

```vue
<template>
	<!-- @keyup.enter 键盘监听，当按下 Enter 键时触发 -->
  <div class="login" @keyup.enter="login(form)">
      <!-- element卡片 -->
    <el-col :span="8">
      <el-card shadow="hover">
          <!-- element表单 |model：表单数据对象，rules：表单验证规则，ref:组件注册，引用的信息将会被注册在父组件的$refs对象上，prop:表单域model字段，在使用validate、resetFields方法的情况下，该属性是必填的-->
          <!-- clearable 属性，使 el-input 输入框可清空，show-password 使输入的内容可隐藏 -->
        <el-form ref="form" :model="form" status-icon :rules="rules" :ref="form" label-width="80px">
          <el-form-item label="账号" prop="username">
            <el-input placeholder="请输入账号" v-model="form.username" clearable></el-input>
          </el-form-item>
          <el-form-item label="密码" prop="password">
            <el-input placeholder="请输入密码" v-model="form.password" clearable show-password></el-input>
          </el-form-item>
          <el-form-item>
            <div class=" loginButton">
              <el-button type="primary" plain @click="login(form)">登录</el-button>
              <el-button @click="resetForm(form)">重置</el-button>
            </div>
          </el-form-item>
        </el-form>
      </el-card>
    </el-col>
  </div>
</template>

<script>
  export default {
    data() {
        // 触发规则，触发会传入 rule value callback，value 就是输入框中的值
      let validateUser = (rule, value, callback) => {
        if (value === '') {
          callback(new Error('请输入账号'));
        }
        callback();
      };
      let validatePass = (rule, value, callback) => {
        if (value === '') {
          callback(new Error('请输入密码'));
        }
        callback();
      };
      return {
        form: {
          username: '',
          password: '',
        },
        rules: {
            // 绑定的表单 model 规则，触发会前往写好的函数中
          username: [
            { validator: validateUser, trigger: 'blur' }
          ],
          password: [
            { validator: validatePass, trigger: 'blur' }
          ],
        }
      }
    },
    methods: {
      login(formName) {
          // valid 当表单中的输入空中有一个框为空时，返回 false
        this.$refs[formName].validate((valid) => {
          if (valid) {
            let data = this.$refs[formName].model
            // 向后端发送请求，并传 username,password 给后端
            this.$http.post("/user/signin", {
              username: data.username,
              password: data.password
            }).then(res => {
              if (res.errcode == 0) {
                  //当请求成功时，获取token值，将token设置在localStorage中
                  // localStorage， localStorage 和 sessionStorage 属性允许在浏览器中存储 key/value 对的数据
                  // localStorage 用于长久保存整个网站的数据，保存的数据没有过期时间，直到手动去删除。
                localStorage.setItem("token", res.data.token)
                this.$http.get('/user/info').then(res => {
                  res => {
                    if (res.errcode == 0) {
                        // 将数据传送给项目中，设置为静态数据
                      this.$store.commit('setUser', res.data)
                    } else {
                      this.router.push("/login")
                    }
                  }
                })
                this.$router.push("/")
              } else {
                this.$message({
                  showClose: true,
                  message: res.errmsg,
                  type: "error"
                });
              }
            })
          }
        });
      },
      resetForm(formName) {
          // 将表单中的所有数据清空
        this.$refs[formName].resetFields();
      }
    },
  }
</script>

<style>
  .login {
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .loginButton {
    display: flex;
    justify-content: space-evenly;
  }
</style>
```

项目的主要功能 用户界面

```vue
<!-- /user/list.vue -->
<template>
  <layout>
    <div class="ctrl">
        <!-- v-model 同步值 -->
      <el-input placeholder="请输入搜索关键字" v-model="key" style="width: 15vw;"></el-input>
      <el-button-group>
        <el-button @click="dialogFormVisible = true">批量修改角色</el-button>
        <el-button @click="$router.push('/user/create')">新增{{htmlName}}</el-button>
      </el-button-group>
    </div>
      <!-- el-table 表格 -->
      <!-- border:表格带纵向边框， @selection-change:当选择项发送变化时触发该事件，selection:表格设置添加多选框 -->
    <el-table :data="tableData" border style="width: 100%" @selection-change="handleSelectionChange">
      <el-table-column type="selection" width="55"></el-table-column>
      <el-table-column prop="id" label="ID"></el-table-column>
      <el-table-column prop="username" label="账号"></el-table-column>
      <el-table-column prop="role" label="角色"></el-table-column>
      <el-table-column prop="nickname" label="姓名"></el-table-column>
      <el-table-column fixed="right" label="操作" width="150">
        <template slot-scope="scope">
          <el-button type="text" size="small" @click="$router.push('/user/permission/' + scope.row.id)">权限</el-button>
          <el-button type="text" size="small" @click="$router.push('/user/edit/' + scope.row.id)">编辑</el-button>
          <el-button type="text" size="small" @click="del(scope.row,scope.$index)">移除</el-button>
        </template>
      </el-table-column>
    </el-table>

	<!-- visible.sync 同 v-model -->
    <el-dialog title="绑定角色" :visible.sync="dialogFormVisible">
      <el-form>
        <el-form-item label="角色选择" label-width="80">
          <el-select v-model="roleId" clearable filterable placeholder="请选择">
            <el-option v-for="(item , label) in permissions" :value="item.id" :label="item.name"></el-option>
          </el-select>
        </el-form-item>
      </el-form>
        <!-- slot="footer" 对话框操作区内容 -->
      <div slot="footer" class="dialog-footer">
        <el-button @click="dialogFormVisible = false">取 消</el-button>
        <el-button type="primary" @click="batch">确 定</el-button>
      </div>
    </el-dialog>

	<!-- 分页选择器 -->
	<!-- current-page:当前页数，@current-change:当current-page改变的时候触发,page-size:每页显示条目个数,page-sizes:每页显示个数选择器的选项设置,@size-change：pageSize改变时候触发，layout：显示布局，total：总条目数 -->
    <div style="text-align: right;">
      <el-pagination @current-change="getData" :current-page="currentPage" @size-change="pageSize" page-size="2"
        :page-sizes="[2,4,6,8]" layout="total, sizes, prev, pager, next, jumper" :total="total">
      </el-pagination>
    </div>
  </layout>
</template>

<script>
  export default {
    data() {
      return {
        tableData: [],
        key: '',
        htmlName: '用户',
        total: 1,
        currentPage: 1,
        pageSizeIndex: 2,
        permissions: [],
        userIds: [],
        roleId: '',
        roleIds: [],
        dialogFormVisible: false
      }
    },
    created() {
      this.getData()
      this.$http.get('/role/select').then(res => {
        if (res.errcode == 0) {
          this.permissions = res.data
        }
      })
    },
    watch: {
      key(key) {
        this.key = key
        this.getData()
      }
    },
    methods: {
      batch() {
        this.$http.post('/user/role/update', {
          roleIds: [this.roleId],
          userIds: this.userIds
        }).then(res => {
          if (res.errcode == 0) {
            this.getData()
          }
        })
        this.dialogFormVisible = false
      },
      pageSize(size) {
        this.pageSizeIndex = size
        this.getData()
      },
      handleSelectionChange(items) {
        this.userIds = items.map(item => item.id)
      },
      getData(page) {
        if (page) {
          this.currentPage = page
        }
        let path = `/user/page?currentPage=${this.currentPage}&pageSize=${this.pageSizeIndex}`
        if (this.key) {
          path = `/user/page?currentPage=${this.currentPage}&pageSize=${this.pageSizeIndex}&key=${this.key}`
        }
        this.$http.get(path).then(res => {
          if (res.errcode == 0) {
            let data = res.data
            this.tableData = data.list
            this.total = data.count
          }
        })
      },
      del(item, index) {
        this.$confirm('此操作将永久删除,是否继续?', '提示', {
          confirmButtonText: '确定',
          cancelButtonText: '取消',
          type: 'warning'
        }).then(() => {
          this.$http.post('/user/trash', {
            id: item.id
          }).then(res => {
            if (res.errcode == 0) {
              this.tableData.splice(index, 1)
            }
          })
        })
      },
    },
  }
</script>

<style>
  .ctrl {
    display: flex;
    justify-content: space-between;
    margin: 15px;
  }
</style>

<!-- /user/save.vue -->
<template>
  <layout>
    <div class="ctrl">
        <!-- $router.back() 返回上一个页面 -->
      <el-page-header @back='$router.back()' :content="title() + htmlName + '页面'"></el-page-header>
    </div>
    <el-form label-width="80px">
      <el-form-item label="账号">
        <el-input v-model="form.username"></el-input>
      </el-form-item>
      <el-form-item label="密码">
        <el-input v-model="form.password"></el-input>
      </el-form-item>
      <el-form-item label="姓名">
        <el-input v-model="form.nickname"></el-input>
      </el-form-item>
      <el-form-item>
        <el-button @click="save">{{buttonName}}{{htmlName}}</el-button>
      </el-form-item>
    </el-form>
  </layout>
</template>

<script>
  export default {
    data() {
      return {
        htmlName: '用户',
        buttonName:'',
        form: {
          username: '',
          password: '',
          nickname: ''
        }
      }
    },
    created() {
      if (this.$route.params.id) {
        this.$http.get(`/user/get?id=${this.$route.params.id}`).then(res => {
          if (res.errcode == 0) {
            this.form = res.data
          }
        })
      }
    },
    methods: {
      save() {
        if (this.$route.params.id) {
          this.$http.post('/user/update', this.form).then(res => {
            if (res.errcode == 0) {
              this.$router.back()
            }
          })
        } else {
          this.$http.post('/user/insert', this.form).then(res => {
            if (res.errcode == 0) {
              this.$router.back()
            }
          })
        }
      },
      title() {
        if (this.$route.params.id) {
          this.buttonName = "编辑"
          return "编辑"
        } else {
          this.buttonName = "新增"
          return "新增"
        }
      }
    },
  }
</script>

<style>
  .ctrl {
    display: flex;
    justify-content: space-between;
    margin: 15px;
  }
</style>
```

