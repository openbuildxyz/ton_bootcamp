# TON 学习记录

## 个人信息

* Github: [metanomad21](https://github.com/metanomad21)

* Wechat ID: think_van

* 钱包地址: 0x02633a67BcB83Ff7e4920f92a4990478B3ACA2c3

## 作业提交

[Task1](https://github.com/metanomad21/tact-template-lesson1-homwwork/lesson1)

修改SampleTactContract合约,增加一个getter方法,重新部署,并调用此新方法
* 新增了getter函数：getOwner
* 调用脚本：sources/contract.read.ts

修改SampleTactContract合约,增加一个消息处理方法,重新部署,并发送此新消息
* 新增了receive函数：decrement
* 调用脚本：sources/contract.write.ts
* 合约地址：kQBUWdjuAFMORI8nd4Nu9963AZLCef-Daesq_rv2FF81gcKe
* 调用decrement：https://testnet.tonviewer.com/transaction/92c68ece937275a2cc09d53d998c5c8a9fb51e1a9c5f7a979172992c450e2146


[Task2](https://github.com/metanomad21/tact-template-lesson1-homwwork/tree/lesson2)

增加 Multiply/Divide 消息，并实现对应的接收处理方法
* 新增消息函数：Sub、Mul、Div
* 源文件：/sources/contract.tact
* 合约地址：EQBFj26lWhIB9hZlL_TgvbLhFcFv7DzB1XbB-Uxgl36YXX1z

通过上一课的ts工程，将合约部署到链上，并向合约随机发送加减乘除指令，在区块浏览器查看交易信息
* 调用脚本：sources/contract.random.ts
* 交易tx:https://testnet.tonviewer.com/transaction/720ec7d0070654d9d8745c70fed50272adb3565b05b759749b8544d628612066

## 学习日志
