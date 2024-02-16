# TON 学习记录

## 个人信息

* Github: [kojhliang](https://github.com/kojhliang)

* Wechat ID: kojhliang 或 18928730318

* 钱包地址(EVM兼容地址): 0xD08920C19F9e81F05CE2e16f8fd7B3C7C6c61C58
  
* 个人介绍：Head of Research at Keneitc Capital 

## 作业提交

### 第一课  
作业要求：  
修改SampleTactContract合约,增加一个getter方法,重新部署,并调用此新方法  
修改SampleTactContract合约,增加一个消息处理方法,重新部署,并发送此新消息  
  
第一课作业代码：[https://github.com/kojhliang/tact-template/blob/main/sources/lesson1_contract.tact](https://github.com/kojhliang/tact-template/blob/main/sources/lesson1_contract.tact)

第一课作业发送自定义消息的交易：https://testnet.tonviewer.com/transaction/5531be6fcda3af384ec37410425daa76a1fb148313d11db8e7d5344750e7cc3a?section=trace

第一课合约地址：https://testnet.tonviewer.com/kQB0hBxIk1vBg3IMlCPN0l-E34I6TvZGsED2w-pD1_Vymcuo

### 第二课  
作业要求：  
增加 Multiply/Divide 消息，并实现对应的接收处理方法  
通过上一课的ts工程，将合约部署到链上，并向合约随机发送加减乘除指令，在区块浏览器查看交易信息  
  
第二课作业合约代码：[https://github.com/kojhliang/tact-template/blob/main/sources/lesson2_contract.tact](https://github.com/kojhliang/tact-template/blob/main/sources/lesson2_contract.tact)

第二课作业合约地址：https://testnet.tonviewer.com/kQChbxcoPb4m15GRHyyMFYgjN1-VD-2MbHhjpXf0QVnMYyPm

第二课作业发送消息(Multiply)：https://testnet.tonviewer.com/transaction/bc27c1c17c65e985afb3ef0d9f36157f4fa712ef7631c1b74d2ae10c7e4ecbfe

第二课作业发送消息(Divide)：https://testnet.tonviewer.com/transaction/8758e9e5e042876a5a567be6ad5b5b6630503146fba43f39f4b7cb06b859bb65

### 第三课  
作业要求：   
修改Jetton合约，每次转账时，都收取1%的手续费，将手续费打到固定地址。如转账100，则实际到账99，手续费收1。  

第三课作业合约代码：[https://github.com/kojhliang/tact-template/blob/main/sources/lesson3_contract.tact](https://github.com/kojhliang/tact-template/blob/main/sources/lesson3_contract.tact)

第三课作业Jetton Master合约地址：https://testnet.tonviewer.com/0QCJGZ_OeWeK-ayBd5lSJnduBiFqPCKmnF6vtYDIFQb13wJO  

第三课作业发送消息(转账一定金额到A地址，同时会把1%的金额转到B地址)：https://testnet.tonviewer.com/transaction/56d57f9592173fc2cbfddb6ba06e11ea1153a13da964b5d2e948b6643d878148  

### 第四课    
作业要求：     
完成一个 NFT 合约，支持替他人 mint，且每个账户最多 mint 3次。 （增加消息和结构体来实现）  
实现原理：  
（NFT集合）合约 --》（NFT集合和用户）合约 --》 （NFT集合和用户和NFT的ITEM）合约  
                   若用户mint次数大于3则回弹  

第四课作业合约代码：[https://github.com/kojhliang/tact-template/blob/main/sources/lesson4_contract.tact](https://github.com/kojhliang/tact-template/blob/main/sources/lesson4_contract.tact)  
  
第四课作业NFT collection合约地址：https://testnet.tonviewer.com/kQDLheptvuOcCQcLKacdTUhv4KWuCVh4uC3ZA3KkLXIOmoaU

  

## 学习日志  
[完成作业过程中的笔记](https://github.com/kojhliang/tact-template/blob/main/Note.md)

[Ton智能合约设计的一些思考](https://medium.com/@kojhliang/ton%E6%99%BA%E8%83%BD%E5%90%88%E7%BA%A6%E8%AE%BE%E8%AE%A1%E7%9A%84%E4%B8%80%E4%BA%9B%E6%B7%B1%E5%BA%A6%E6%80%9D%E8%80%83-9e8dae3a5e7b)
