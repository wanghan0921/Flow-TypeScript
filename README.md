# JavaScript语言特征介绍

JavaScript是一种弱类型的, 动态类型检查的语言

 
## 弱类型 和 强类型

### 弱类型

  在定义变量的时候, 我们可以为变量赋值任何, 变量的数据类型不是固定死的, 这样的类型的叫做弱类型
  
  ```JavaScript
  var a = '123'
  a = 10
  a = () => {}
  ```
  
### 强类型

  在声明变量时, 一单给变量赋值, 那么变量的数据类型就已经确定了, 之后如果要给变量赋值其他类型的数据, 需要进行强制数据类型转换

  ```java
  int a = 10
  ```
  
## 动态类型 和 静态类型

动态类型和静态类型的核心区别: 动态类型的类型检查会在代码运行的时候进行, 而静态类型的类型检查则是在编译时进行

运行时检查
```JavaScript
var obj = {}
obj.forEach(item => {
  
})
```

编译时检查
```java
int num = 10
num = "123"
```

## 动态类型 可能会带来的问题

  代码中的错误, 只能在代码运行的时候被发现
  
  测试阶段, 也许有的问题可以测试出来, 但有的问题没有测试出来, 当项目上线后, 报错. 代码不稳定
  
  好处: 编码简单且方便


## 静态类型的优势

 ### 提早发现代码中的bug
 
 ```js 
 function greet(obj){
  obj.sayHi()
 }
 
 var o = {
  name: 'wanghan'
 }
 
 greet(o)
 ```
 
 ### 提高代码的可读性
 
 ```js
 // 如果能指定a和b的类型
 // 指定为数字, 这个函数的功能就非常明确了
 function(a, b) {
  return a + b
 }
 ```
 
 ### 减少了复杂的错误处理逻辑
 
 ### 便于代码重构






























