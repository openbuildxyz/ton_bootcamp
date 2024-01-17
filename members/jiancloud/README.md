
# TON 学习记录

## 个人信息
* Github: [云风](https://github.com/jiancloud)
* Wechat ID: jiancloud
* ETH系钱包地址: 0xC1716C8f2742f9f645111A62f9730f32F9B101b0

## 作业提交

### 作业一
***部署在测试网的合约地址***：  
https://testnet.tonviewer.com/kQC-R_VHe-yDX90h1gQjwPDoYK5gqRcJKnxl5b2Alh-0tc48  
https://verifier.ton.org/EQC-R_VHe-yDX90h1gQjwPDoYK5gqRcJKnxl5b2Alh-0tXW2?testnet  

***作业一代码*** ：   
https://github.com/jiancloud/tact-template-main

### 作业二
***部署在测试网的合约地址***：  
https://testnet.tonviewer.com/kQAKxDq0wJI8SGbAvbBvtHCrO8CoraioNlvkIBMB9YYG8L2y   
https://verifier.ton.org/tactDeployer/QmfXf1umkR7JwhFRHK65vc7JMoaX4mV64NeCsnbMDUGTCe?testnet    
***作业二代码***：  
https://github.com/jiancloud/tact-template-main/tree/lesson2

## 学习日志

### 作业一
#### 1 TON生态
- Telegram于 2018 年创建了 Telegram Open Network
- 在 Telegram 放弃 TON 项目后，一群社区开发人员将其重新命名为 The
  Open Network
- Telegram App整合自托管钱包“Ton Space”，支持TON钱包
- 2023年 9 月，Telegram 已认定选择 TON 网络作为其 Web3 基础设施的区块
  链网络，TON 生态的多个项目和进展都将基于 Telegram 进行构建
- TON 背靠 Telegram 的 8 亿多用户支持，有着类似微信的发展前景
#### 2 Tact语言
> TON 生态系统主要使用两种智能合约编程语言：FunC 和 Tact。
- FunC 是一种低级语言，专为深入了解 TON 架构的开发人员而设计，它在开
  发复杂的多合约系统时可能具有挑战性。
- Tact 是 TON 区块链的一种新编程语言，注重效率和简单性。它的设计易于学
  习和使用，并且非常适合智能合 约。 Tact 是一种静态类型语言，具有简单的语
  法和强大的类型系统。
- Tact 提供了受 JavaScript 和 Typescript、Rust 和 Swift 启发的熟悉语法。对于
  新开发人员来说，代数数据类型和编译时执行等强大功能看起来有机且友好。
- 编译器会把Tact代码转译为FunC代码，最终编译为类似Fift的字节码，在TON
  VM虚拟机上执行。
#### 3 Tact开发环境搭建
- 安装TON钱包
- 创建区块链账户
- 配置测试区块链网络
- 申领测试币
- 安装Visual Studio Code插件Tact Language Support
#### 4 智能合约示例
- 合约说明
1. 从模版工程开始 git git@github.com:tact-lang/tact-template.git
2. 一个示例合约SampleTactContract
3. 具备状态：owner和counter
4. 初始化函数：init
5. 合约方法：add
6. 消息处理函数：可处理两种类型消息
7. getter方法：counter
- 配置说明
1. 在tact.config.json文件中配置源文件和输出目录
2. 在package.json文件中配置编译命令
3. 执行命令 yarn build 编译
- 部署说明
1. 导入相关的TS库
2. 准备合约参数
3. 准备部署合约
4. 计算合约地址
5. 合约部署网址
6. 浏览器打开网址
7. 钱包签名部署
8. 浏览器查看已部署合约
- 合约调用说明：调用getter
1. 导入TON的开发库
2. 准备合约参数
3. 调用getCounter读取状态值
- 发送消息
1. 导入TON的开发库
2. 准备合约参数
3. 调用send方法发送消息
#### 5 总结
- TON生态背靠Telegram
- TON的合约语言有FunC和Tact
- 在TON上操作，需要钱包和TON代币，开发时建议使用TON测试网络
- Tact开发环境搭建
- Tact Helloworld合约编写，编译、部署、和调用

#### 6 参考资料
- https://docs.ton.org/
- https://tact-lang.org/
- https://github.com/tact-lang/awesome-tact
- https://docs.tact-lang.org/
- https://ton.app
- https://foresightnews.pro/article/detail/21329
- https://www.fx168news.com/article/392979
- https://www.panewslab.com/zh/articledetails/ty2spsyy.html
- https://www.techflowpost.com/article/detail_14664.html

### 作业二
#### Tact基本结构
* 可以从其他合约 import 导入现有合约
* 新的合约以 contract 关键字开始
* 可以使用 with 关键字从其他 trait 继承
* 有私有变量，可存储合约状态
* 有初始化函数 init 用于初始化合约状态
* 可以 self 关键字访问当前合约的状态和方法
* 可定义方法函数
#### 原始类型
* Int - Tact 中的所有整数都是 257 位有符号整数
* Bool - 具有真/假值的经典布尔值
* Address 标准地址
* Slice、Cell、Builder - TON VM 的低级原始类型
* String - 表示 TON VM 中文本字符串的类型
* StringBuilder - String工具类型，可以高效的方式连接字符串
#### 结构体和消息
* struct 关键字定义结构体类型
* message 关键字定义消息类型
* 结构体和消息几乎是相同的 东西，唯一的区别是消息在其序列化中具有标头，因此可以用作接收器
#### 字典
* 类型 map<k, v> 用于将数据与相应的键关联起来
* Possible key types: 可能的key类型：
  * Int 整数
  * Address 地址
* Possible value types: 可能的value类型
  * Int 整数
  * Bool 布尔值
  * Cell Cell（TON特有的数据类型，最多1023bit以及最多4个其他Cell的引用）
  * Address 地址
  * Struct/Message 结构/消息
#### Contract 合约
* 合约是 TON 区块链上智能合约的主要入口。它包含合约的所有状态、函数、获取者和接收者。
#### Trait 特征
* Tact 不支持经典的类继承，而是引入了trait的概念，合约可以从Trait继承
* Trait 定义了函数、接收者和必填字段
* Trait 就像抽象类，但它没有定义字段的存储方式和位置
  * Trait的所有字段都必须在合约本身中明确声明
  * Trait本身也没有构㐀函数，所有初始字段初始化也必须在主合约中完成
#### 运算符
* ! 逻辑反转，仅为 Bool 类型定义
* / 、 * 、 % 除法、乘法和取模运算， 仅为 Int 类型定义
* \- 、 + 算术运算，仅为 Int 类型定义
* != 、 == 相等运算
* \> 、 < 、 >= 、 <= 比较操作，仅为 Int 类型定义
* && 、 || 逻辑 AND 和 OR
* !! 后缀运算符 - 强制执行非空值，仅为可空类型定义。大多数原始类型、结构体和消息都可以为空
* initOf 计算合约的初始状态
#### 常量
* 简单常量，它是在编译时定义的值，无法更改。可以在顶层或contract/trait内定义常量
* 虚拟常量是可以在trait中定义但在contract中更改的常量。当您需要在编译时配置某些trait时，它非常有用
* 抽象常量是可以在trait中定义但不指定值的常量
#### If 语句
* if
* if/else
* if/else if/else
#### Repeat循环
* 重复循环执行一段代码指定的次数
  * 重复数必须是32位int，否则会抛出超出范围的异常。负值将被忽略。
#### While循环
* 只要给定条件为真，While 循环就会继续执行代码块
```tact
let x: Int = 10;
while(x > 0) {
  x = x -1;
}
```
#### Until循环
* Until 循环是一个测试后循环，它至少执行一次代码块，然后继续执行直到给定条件成立
```tact
let x: Int = 10;
do {
  x = x - 1;
} util (x <= 10);
```
#### 函数及其类型
> Tact 中的函数可以用不同的方式定义
* Global static function 全局静态函数
  > 可以在程序中的任何位置定 义全局函数
  ```tact
    fun pow(a: Int, c: Int): Int {
      let res: Int = 1;
      repeat(c) {
        res = res * a;
      }
      return res;
    }
  ```
* Extension functions 扩展功能
  > 扩展函数由关键字 extends 修饰，允许对任何类型进行扩展。  
  *第一个参数的名称必须命名为 self，并且此参数
  的类型是要扩展的类型*
  ```tact
  extends fun pow(self: Int, c: Int) {
    let res: Int = 1;
    repeat(c) {
      res = res * self;
    }
    return res;
  }
  let some: String = 95.toString(); // toString() is a stdlib function
  ```
* Mutable functions 可变函数
> 可变函数是指可以改变self值的扩展函数
```tact
extends mutates fun pow(self: Int, c: Int) {
  let res: Int = 1;
  repeat(c) {
    res = res * self;
  }
  self = res;
}
```
* Native functions 原生函数
> 原生函数是指直接绑定到 func的函数  
> 原生函数也可以是可变和扩展的。
```tact
@name(store_unit)
native storeUnit(s: Builder, value: Int, bits: Int): Builder;
@name(load_int)
extends mutates native loadInt(self: Slice, l: Int): Int;
```
* Receiver functions 接收器功能
> 接收器函数是负责接收合约中消息的特殊函数，只能在contract或trait中定义。
```tact
contract Treasure {
  // ...
  
  receive("increment") {
    self.counter = self.counter + 1;
  }
}
```
* Getter functions 读取函数
> Getter 函数在智能合约上定义 getter，并且只能在contract或trait中定义。
```tact
contract Treasure {
  // ...
  get fun counter() {
    return self.counter;
  }
}
```
#### 消息类型
> TON合约之间的通信是通过发送和接收消息来完成的。    
> TON 区块链是一种基于消息的区块链，可与您需要发送消息的其他合约进行通信。
* 消息分为两种
  * 内部消息：最常见的消息类型是内部消息 - 从一个合约（或钱包）发送到另一个合约的消息
  * 外部消息：外部消息是与链下系统集成的，一般开发中较少遇到，本教程中不做深入学习
* 接收内部消息
  > 一个合约允许定义有多个接收器函数。所有接收器函数都按照下面列出的顺序进行处理：
  * receive() - 当向合约发送空消息时调用
  * receive("message") - 当带有特定文本的消息发送到合约时调用
  * receive(str: String) - 当任意文本消息发送到合约时调用
  * receive(msg: MyMessage) - 当 MyMessage 类型的二进制消息发送到合约时调用
  * receive(msg: Slice) - 当未知类型的二进制消息发送到合约时调用
* 消息组成  
  消息本身由如下部分组成：
  * value in TON - 您想要与消息一起发送的TON数量。该值用于支付接收方的 Gas 费。
  * bounce - 如果设置为 true （默认），那么如果接收者合约不存在或无法处理消息，消息将被退回 给发送者。
  * code 和 data - init 包，对于部署很有用。
  * body - 消息正文为 Cell。
  * mode - 配置如何发送消息的 8 位标志。
* 使用reply发送简单消息  
  最简单的消息是对传入消息的回复，并返回消息的所有的TON代币余值：
  ```tact
  self.reply("Hello, World".asComment());
  ```
* 使用send发送消息
  * 如果需要自定义发送消息参数，可以使用 send 函数。
  * 如下代码表示向 to 地址发送一条消息，其中 value 为 1 TON， body 为字符串“Hello, World!”的文本。  
  *SendIgnoreErrors 意味着即使在消息发送过程中发生错误，下一条消息仍然会被发送。*
  ```tact
    let to: Address = ...;
    let value: Int = ton("1");
    send(SendParameters{
      to: to,
      value: value,
      mode: SendIgnoreErrors,
      bounce: true,
      body: "Hello, world".asComment()
    });
  ```
* 发送自定义结构体消息  
  要发送二进制类型的消息，您可以使用以下代码：
  ```tact
    let to: Address = ...;
    let value: Int = ton("1");
    send(SendParameters{
      to: to,
      value: value,
      mode: SendIgnoreErrors,
      bounce: true,
      body: SomeMessage{arg1: 123, arg2: 1234}.toCell()
    });
  ```
* 发送部署合约消息  
  要部署合约，您需要计算它的地址和初始化包，然后将其与初始消息一起发送。您始终可以发送带有消息的 init 包，它会被忽略，但比没有 init 包的消息花费更多。  
  ```tact
    let init: StateInt = initOf SecondContract(arg1, arg2);
    let address: Address = contractAddress(init);
    let value: Int =  ton("1");
    send(SendParameters{
      to: address,
      value: value,
      mode: SendIgnoreErrors,
      bounce: true,
      code: init.code,
      data: init.data,
      body: "Hello, world".asComment()
    });
  ```
* 处理bounced消息
  * 当合约发送一条消息，并将反弹标志(bounce)设置为true 时，如果该消息未正确处理，它将反弹回发送者。 发送者可以做一些补救操作，比如回滚。
  * bounced消息有些限制，比如不支持文本消息，且消息大小目前不超过224bits。  
  bounced消息处理函数定义:  
  ```tact
    contract MyContract {
      bounced(src: bounced<MyMessage>) {
        // ...
      }
      bounced(src: Slice) {
        // ...
      }
    }
  ```
* 内置函数
  > 主要有Common、Strings、Random、Math、Cells、 Builders、Slices  
  > Refer https://docs.tact-lang.org/language/ref/common  
  
  示例：  
  * fun sender(): Address;
  * fun require(condition: Bool, error: String);
  * fun now(): Int
  * fun myBalance(): Int;
  * fun myAddress(): Address;
  * fun ton(value: String): Int;
  * fun context(): Context;
* 标准库
  > 标准库也封装了一些traits，合约直接继承可用
  > Refer https://docs.tact-lang.org/language/libs/deploy
#### 总结
* Tact语言比较简洁，类似于JavaScript的语法，能够快㏿上手。
* 专为TON区块链设计，可编译为FunC语言。
