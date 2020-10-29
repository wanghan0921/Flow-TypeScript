# ts配置文件

1. 生成ts配置文件
```shell
tsc --init
```

2. 设置配置项
  * target: 指的就是将ts代码转化成哪个版本的js代码 es5 es3
  * module: 指的就是将ts代码转换成js代码之后, 使用的模块化的标准是什么
  * outDir: 指的就是将ts代码转化成js代码以后, js代码的存放路径
  * rootDir: 指的就是要将那个目录中的ts文件进行转码, ts代码的存放了路径
  * strict: 是否要将ts代码转化成严格模式的js代码
  
3. 使用配置文件
```shell
tsc -p ./tsconfig.json
```































