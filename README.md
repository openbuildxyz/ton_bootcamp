# OpenBuild 公开课系列｜TON 开发从入门到应用

Hi, 感谢大家报名此次 OpenBuild 公开课系列，关于本次的详情请查看此文章：[OpenBuild 公开课系列｜TON 开发从入门到应用](https://mp.weixin.qq.com/s?__biz=MzU4Mjk1MTI2NA==&mid=2247489282&idx=1&sn=1691dd397a26272f0319279894aa06b2&chksm=fdb1df0dcac6561bd459482fc68dbfdc25ef02ac36f609b59b5500e4583175019faca83a7b23#rd)

本 Repo 主要有以下作用：

1. 每次课程结束后，会设立 Coding Challenge，开发者完成后需要通过 PR 提交到这个仓库里，**完成的开发者将获得由 TON 基金会发放的 Bounty 奖励**
2. 为大家更新 TON 学习的一些材料，帮助大家更好的学习 TON 应用开发，同时也欢迎大家提交好的学习资料，积极贡献的开发者也将获得 Bounty 激励
3. 学习中遇到的任何问题，也欢迎通过 issue 提交，我们会帮助解答

**如果你还没报名，请 [点此报名](https://openbuild.xyz/learn/challenges/2023609337)，我们将在课程结束后为参与学习和产出的开发者颁发对应 NFT 证书和勋章，贡献优异的开发者同时将获得 OpenBuild 的 SBT，后续将享受一系列社区权益**。

### 目录

1. TON 开发从入门到应用
2. Coding Challenge 及奖励说明
3. TON 学习资源

## TON 开发从入门到应用
- 第一节 视频[TON&Tact](https://openbuild.xyz/learn/challenges/2023609337)  文档 [TON&Tact Intro](https://github.com/0xOutOfGas/tact-learning)  代码[tact-template](https://github.com/0xOutOfGas/tact-template)
- 第二节 视频[Tact语法概述](https://openbuild.xyz/learn/challenges/2023609337/2936) 文档 [Tact语法概述](https://github.com/0xOutOfGas/tact-learning)  代码[receivers](https://tact-by-example.org/03-receivers)
- 第三节 视频[FT标准介绍与实战](https://openbuild.xyz/learn/challenges/2023609337/2937) 文档 [FT标准介绍与实战](https://github.com/0xOutOfGas/tact-learning)   代码[receivers](https://github.com/howardpen9/jetton-implementation-in-tact)
- 第四节 视频[NFT标准介绍与实战](https://openbuild.xyz/learn/challenges/2023609337/2938) 文档 [NFT标准介绍与实战](https://github.com/0xOutOfGas/tact-learning)   
- 第五节 视频[Tact合约测试和交互](https://openbuild.xyz/learn/challenges/2023609337/2939) 文档 [Tact合约测试和交互](https://github.com/0xOutOfGas/tact-learning)   
- 第六节 视频[Tact安全实践](https://openbuild.xyz/learn/challenges/2023609337/2940) 文档 [Tact安全实践](https://github.com/0xOutOfGas/tact-learning)   

## Coding Challenge 及奖励说明
### 如何提交作业
Fork 本仓库，复制 members/githubid 目录名为 [members/$your_github_id](https://github.com/openbuildxyz/ton_bootcamp/tree/main/members/your_github_id)，根据自己的信息编辑其中的 readme.md 内容，并提交 Pull Request 给本仓库，报到成功。

### 奖学金计划
为了防止女巫，以上活动参与的人必须注册和完善 OpenBuild https://openbuild.xyz/ 的 Profile，且必须绑定 Github和钱包地址。（不绑定 github 和钱包则没有奖励）
- 🏅 阶段一 10U
  - 完成作业一
    - 修改SampleTactContract合约,增加一个getter方法,重新部署,并调用此新方法
    - 修改SampleTactContract合约,增加一个消息处理方法,重新部署,并发送此新消息

- 🎖 阶段二 20U
  - 完成作业二
    - 增加 Multiply/Divide 消息，并实现对应的接收处理方法
    - 通过上一课的ts工程，将合约部署到链上，并向合约随机发送加减乘除指令，在区块浏览器查看交易信息
  - 完成作业三
    - 修改Jetton合约，每次转账时，都收取1%的手续费，将手续费打到固定地址。如转账100，则实际到账99，手续费收1。 

- 🏆 阶段三 30U
  - 完成作业四
    - 完成一个 NFT 合约，支持替他人 mint，且每个账户最多 mint 3次。
  - 完成作业五
  - 完成作业六

- 🌈成为贡献者 & Maintainer 10-200U
  - 发布 TON 相关的学习笔记[文章或者视频]
  - 成为社区TON大使，为TON生态做技术布道师
  - 对 TON 生态项目有 PR 贡献，mentor 会评估 PR 的复杂度
  - 开发出具有创新性的TON应用(团队或个人）
  - Maintainer需主持至少一次 Office Hour [可联系微信：sqiuqiu999]
  - 以上5项需要满足一项

- 🎁神秘大奖
  - 对贡献最多的团队或个人奖励神秘大礼


### TON 学习资源

#### 教程类

1. [TON 官方文档](https://docs.ton.org/)
1. [Tact 官方开发文档](https://docs.tact-lang.org/)
1. [TON 亚太开发者共学营课程](https://openbuild.xyz/learn/courses/99): 想要深入区块链的奇妙世界，成为 TON 生态系统的专家吗？来加入 TON x BuidlerDAO 的技术课程，打开区块链知识和技能的大门吧

#### 工具类

1. [awesome-ton](https://github.com/ton-community/awesome-ton): A curated list of remarkable libraries, tools, services, protocols, and smart contracts related to TON.

2. [ton faucet bot](https://t.me/testgiver_ton_bot): A TON Blockchain Testnet Faucet Bot
