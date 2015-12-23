
# Penny 文档

## 简介

```php
print("Hi,Penny!");
```

这是一门类似于`JavaScript` 与 `python`的弱类型语言。

面向于编程语言初学者，通过严格的语法、宽松的风格，使初学者养成良好的编程习惯的同时，亦能够在编程中体会到快乐。

或许，后者才是最主要的原因。因为在开发这门语言的时候，我沉醉其中，只想快乐。

## 注释
`Penny` 不会执行注释。

我们可以添加注释对`Penny`进行注释，以便提高代码的可读性。

注释以 `#` 开头

**例子**
```php
# 我是一行注释
# print("Hello World!");
print("Hi,Penny!"); 
```

## 变量

使用 `var` 声明变量。  

```php
var x = 0;
var y = 1;
```

 `Penny` 允许将函数的返回值作为变量赋值。

```php
function hi(name) {
	return "Hi," + name);
}
var x = hi("Penny");
print(x);

# 打印：Hi,Penny

```

> **注意：**
> `Penny 1.0` 声明变量的时候必须初始化。
> `Penny 1.0` 不允许在一个语句声明多个变量。

**例如，以下的语法都是错误的：**

```php
# 错误1：没有初始化变量
var x;

# 错误2：在同一语句中声明了多个变量
var x = 0, y = 0;
```


## 数据类型
`Penny` 为弱类型语言，拥有动态类型。

具体有`整型`，`浮点型`，`字符串`，`布尔型`。

```php
# x 为整型
var x = 6;

# x 为浮点型
var x = 12.13；

# x 为字符串类型
var x = "Penny";

# x 为布尔型
var x = true;
var y = false;
```

> **注意：**
> `Penny 1.0` 不支持数组类型。


## 函数

函数语法如下，支持传入多参数：
```php
# 函数声明
function functionName(argument1, argument2) {
	# 这里是要执行的代码
}
```

函数调用语法如下：
```php
# 函数调用
functionName(argument1, argument2);
```

函数支持返回值，使用关键字`return`表示
```php
# 函数声明
function myFunction(a, b) {
	return a * b;
}

# 函数调用和赋值
var c = myFunction(5, 6); 
print(c);	
# 打印：30
```

> **注意：**
> `Penny 1.0` 不支持面向对象。

## 控制语句
`Penny 1.0` 支持基本的控制语句：

* `if...else`条件判断语句
* `for`循环语句
* `while`循环语句。

### if 语句
```php
if(a > 12.13) {
	print("Good Bye!");
} else if (a < 12.13 && a >= 11.13) {
	print("Hello!");
} else {
	print("Nothing!");
}
```

> **注意：**
> `Penny 1.0` 不支持单目运算符，所以不可以使用类似于`i++`的语法。


### for 语句
```php
for(var i = 0; i <1000; i = i + 1) {
	print("I miss U！");
}
```

### while语句
```php
var i = 0;
while(i < 1000) {
	print("I miss U!");
	i = i + 1;
}

```


## 运算符

### 逻辑运算符
* 与运算`&&`
* 或运算`||`

### 算数运算符
* `+`
* `-`
* `*`
* `/`
* `%`

### 比较运算符
* `>`
* `>=`
* `<`
* `<=`
* `==`
* `!=`

## 转义符
* 换行：`\n`

## 内置函数
* `print()`
