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
