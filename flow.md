# flow的基本使用

## 安装

```shell
npm init
npm i flow-bin -D
```

## 书写代码, 为代码添加类型

```js
var 变量: 数据类型 = 数据
```

1. 通过注释的方式进行添加 (不会修改js代码, 代码在添加完类型后仍然可以正常运行)
2. 通过直接写js代码结构(推荐) , 改写js代码, 如果要正常运行, 需要使用babel降级

## 使用flow进行类型检查

1. 在package.json文件中, scripts属性中添加flow

2. 需要为flow创建一个配置文件.flowconfig
```shell
npm run flow init
```

3. 执行类型检查
```shell
npm run flow
```


## 使用babel对flow代码进行转码

如果给数据添加类型声明是通过第二种方式, 直接修改js代码, 那么代码是不能正常运行的 

我们需要通过babel对代码进行转码之后才能正常运行

1. 安装babel 以及 presets
```shell
npm i babel-cli babel-preset-flow -D
```

2. 配置package,json添加build命令调用babel
```json
"scripts": {
  "build": "babel ./src -d ./dist"
}
```
3. 执行build命令对文件进行转换













