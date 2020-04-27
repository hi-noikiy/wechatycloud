# demo

[![Powered by Wechaty](https://img.shields.io/badge/Powered%20By-Wechaty-green.svg)](https://github.com/chatie/wechaty)
[![Wechaty开源激励计划](https://img.shields.io/badge/Wechaty-开源激励计划-green.svg)](https://github.com/juzibot/Welcome/wiki/Everything-about-Wechaty)

这是wechatyCloud的Demo演示版。

wechatyCloud是基于wechaty的云平台，最大特点是可以在线安装插件，以实现低代码甚至0代码开发的目的。

下面是demo版本与普通版本的区别：

| 功能 | demo 版本 | 正常版本 | 专业版本 | 企业版本 |
| ---- | ---- | ---- | ---- | ---- |
| 最大用户数量 | 1| 100 | 2000| 50000|
| 沙盒运行插件 | ✔| ✔ | ✔| ✔| ✔|
| 在线编写插件 | ✔| ✔ | ✔| ✔| ✔|
| 在线发布插件 | ✗| ✔ | ✔| ✔| ✔|
| 在线安装插件 | ✗| ✔ | ✔| ✔| ✔|
| 可装插件数量 | 1| 10 | 2000| 无限|
| 掉线自动登录 | ✗| ✔ | ✔| ✔| ✔|

## 架构

采用沙盒机制，用沙盒运行插件。默认的插件，是一个echo。代码在msg.sandbox.js里。

web提供一个按钮，用于在线启动，停止。

web提供一个在线编辑器，可编辑 msg.sandbox.js 文件。保存后，即可生效，无需重新启动wechaty。

## 运行环境

1、linux操作系统，我的是 Linux Mint 19.3

2、node环境，我的node 版本是：10.19.0

3、开启redis服务

## 安装

```
git clone https://github.com/wechatycloud/demo.git
cd demo
npm install
```

## 配置

文件 conf.yml

把 your_puppet_padplus_token 替换成你的token
```
token: your_puppet_padplus_token
port: 3000
botname: wechaty
```

## 启动
```
npm start
```

## 体验

打开浏览器，输入:

http://你的服务器ip:3000

## 关于作者

cr4fun，一个不务正业的产品经理，喜欢用中性笔在纸巾上画原型图，并且常常原型图只画一半就忍不住动手去写代码。

## 致谢

感谢 wechaty 项目组

感谢 句子互动

感谢李佳芮 李卓桓 李云军 ，这几位大牛编著的《Chatbot从0到1》给了我很多启发。
