# solana-awesome

一个为所有对学习和构建 Solana 感兴趣的人提供的全面、真实的资源中心

- [Solana 简介](#solana-简介)
- [Solana 基础](#solana-基础)
- [开发者资源](#开发者资源)
  - [通用学习资源](#通用学习资源)
  - [Anchor 开发](#anchor-开发)
  - [非 Anchor 程序开发](#非-anchor-程序开发)
  - [测试程序](#测试程序)
  - [程序安全](#程序安全)
  - [Crates 和 SDK](#crates-和-sdks)
  - [开发工具](#开发工具)
  - [浏览器](#浏览器)
  - [性能仪表板](#性能仪表板)
  - [游戏](#游戏)
- [压缩](#压缩)
- [Solana 移动端](#solana-移动端)
- [Solana 支付](#solana-支付)
- [验证者](#验证者)
  - [Agave 客户端](#agave-客户端)
  - [Firedancer](#firedancer) 
  - [更新](#更新)
  - [结构](#结构)
  - [运营、维护与经济学](#运营-维护和经济学)   
- [观点和文章](#观点和文章)
- [Solana 的未来](#solana-的未来)

## Solana 简介

| 标题                                                                 | 类型    | 作者       | 链接                                                                                                           | 描述                                                                         |
|-----------------------------------------------------------------------|---------|--------------|----------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| Solana 架构新手指南                                                   | 文章    | Anvit Mangal | [链接](https://anvit.hashnode.dev/a-dummys-guide-to-solana-architecture)                                       | Solana 架构的总体概述                                                              |
| 那么 Solana 到底是怎么回事                                           | 文章    | hana         | [链接](https://2501babe.github.io/posts/solana101.html)                                                        | 对 Solana 基础知识的一种有趣的视角，适合技术读者                                                   |
| 在 Solana 上编程 - 简介                                               | 文章    | Paul X       | [链接](https://paulx.dev/blog/2021/01/14/programming-on-solana-an-introduction/)                               | 对在原生 Rust 中进行 Solana 编程的介绍                                                               |
| Solana：单体                                                         | 文章    | Ceteris      | [链接](https://members.delphidigital.io/reports/solana-the-monolith#more-than-just-scaling-with-hardware-bda3) | Delphi Digital 对 Solana 的全面深入研究                                                                  |
| Solana：工作原理 - Solana 协议的执行概述                               | 报告  | Lostin       | [链接](https://www.helius.dev/blog/solana-executive-overview)                                                  | Solana 核心协议的整体概述。                                                                  |
| Solana 编程模型：Solana 开发简介                                       | 文章    | 0xIchigo     | [链接](https://www.helius.dev/blog/the-solana-programming-model-an-introduction-to-developing-on-solana)       | 关于 Solana 架构、账户模型和交易的介绍性文章                                                         |

## Solana 基础

| 标题                                                                 | 类型       | 作者             | 链接                                                                                                                   | 描述                                                                                                                               |
|-----------------------------------------------------------------------|------------|-------------------|------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| 使 Solana 成为第一个 Web 规模区块链的 8 项创新                             | 文章    | Anatoly Yakovenko | [链接](https://medium.com/solana-labs/7-innovations-that-make-solana-the-first-web-scale-blockchain-ddc50b1defda)      | Solana _modus operandi_ 的八项关键技术概述        |
| Solana 共识                                                         | 文章    | Ryan Chern        | [链接](https://www.helius.dev/blog/consensus-on-solana)                                                                | 一篇阐明历史证明在 Tower BFT（Solana 的共识机制）的插槽中的作用的文章                                                                  |
| Solana 交易的生命周期                                                 | 文章    | Umbra Research    | [链接](https://www.umbraresearch.xyz/writings/lifecycle-of-a-solana-transaction)                                       | Solana 运行时如何处理交易以及 Solana 和 Ethereum 上的交易执行之间的差异的概述                                                                |
| Solana 上的本地费用市场                                               | 推文     | 7Layer            | [链接](https://x.com/7LayerMagik/status/1615569374647287808)                                                           | 一个解释 Solana 区块空间结构的 Twitter 帖子，阐明了费用市场是什么、它们如何工作以及为什么它们有用                                          |
| 优先级费用：了解 Solana 的交易费用机制                                   | 文章    | 0xIchigo          | [链接](https://www.helius.dev/blog/priority-fees-understanding-solanas-transaction-fee-mechanics)                      | 了解 Solana 的交易费用机制、优先级费用以及如何以编程方式实现它们                                                                       |
| Solana 费用                                                         | 文章    | Umbra Research    | [链接](https://www.umbraresearch.xyz/writings/solana-fees-part-1)                                                      | 了解当今 Solana 的费用如何运作                                                                                                             |
| Solana 内部原理                                                      | 文章   | Sec3              | [链接](https://www.sec3.dev/blog/solana-internals-part-1-what-are-the-native-on-chain-programs-and-why-do-they-matter) | 一个深入探讨 Solana 内部原理的 4 部分系列，适合技术读者                                                                                  |
| Solana 节点 - Solana RPC、验证器和 RPC 提供商入门                                | 文章    | Mert Mumtaz       | [链接](https://www.helius.dev/blog/solana-nodes-a-primer-on-solana-rpcs-validators-and-rpc-providers)                  | 了解 Solana 节点、不同类型、它们的重要性以及顶级 RPC 提供商                                                                              |
| Solana 权益证明 + 历史证明入门                                           | 文章    | Shinobi Systems   | [链接](https://www.shinobi-systems.com/primer.html)                                                                    | 深入探讨历史证明 (PoH) 是什么以及它是如何工作的，适合技术读者                                                                                   |
| Solana 的海湾流：无内存池，问题多多                                       | 文章   | Lostin           | [链接](https://www.helius.dev/blog/solana-gulf-stream)                                                                  | 对海湾流（Solana 的无内存池交易转发协议）的探索                                                                                              |
| 股权加权服务质量：您需要了解的一切                                     | 文章    | 0xIchigo          | [链接](https://www.helius.dev/blog/stake-weighted-quality-of-service-everything-you-need-to-know)                      | 了解 SWQoS、Solana 如何处理交易以及验证器和股权日益增长的重要性                                                                           |
| Solana 白皮书                                                        | 白皮书 | Anatoly Yakovenko | [链接](https://solana.com/solana-whitepaper.pdf)                                                                       | Solana 的圣经文本                                                                                                                        |
| 关于 Solana 本地费用市场的真相                                           | 文章    | Lostin            | [链接](https://www.helius.dev/blog/solana-local-fee-markets)                                                           | 本文对 Solana 当前本地费用市场的状态以及需要改进的地方进行了通俗易懂的分析。                                                                   |
| Turbine：Solana 上的区块传播                                            | 文章    | Ryan Chern        | [链接](https://www.helius.dev/blog/turbine-block-propagation-on-solana)                                                | 了解 Solana 上的区块传播、它与 Ethereum 的比较以及区块传播和数据可用性的未来研究途径                                                            |
| 了解 Solana 上的Slot、Block和Epoch                                       | 文章    | Mert Mumtaz       | [链接](https://www.helius.dev/blog/solana-slots-blocks-and-epochs)                                                     | 深入探讨 Solana Slot、Block和Epoch如何协同工作
| Solana 代币扩展入门                                                     | 文章    | Yash Agarwal      | [链接](https://blog.superteam.fun/p/primer-on-solanas-token-extensions)                                                | 深入探讨 Solana 令牌扩展 (Token 2022)，探索它们的用例，以及它们为何可能成为 Solana 令牌化叙事的下一个主要催化剂。 |

## 开发者资源

### 通用学习资源

| 标题                                         | 类型      | 作者       | 链接                                                                            | 描述                                                                                                                   |
|------------------------------------------|---------------|---------------|---------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| 60 天 Solana                                | 教程      | Rareskills    | [链接](https://www.rareskills.io/solana-tutorial)                               | 一个为具有 Ethereum 或 EVM 开发的初级或中级背景的工程师设计的 60 天 Solana 课程                                               |
| 从头开始创建一个 Solana dApp                     | 教程      | Loris Leiva   | [链接](https://lorisleiva.com/create-a-solana-dapp-from-scratch)                | 一个关于构建简化版 Twitter 作为 Solana dApp 的系列                                                                  |
| Rust + Solana 高级开发课程                       | 教程      | ICB           | [链接](https://careerbooster.io/courses/rust-solana-advance-development-course) | 一个免费的高级 Solana 开发课程                                                                                             |
| Solana Bootcamp                          | 视频         | Solana Foundation | [链接](https://youtu.be/0P8JeL3TURU?si=jl41rZ5Nrfx3O-Im)                        | 一个视频海盗主题训练营，用于快速掌握 Solana 编程                                                                     |
| Solana Bytes                             | 视频         | Solana Foundation | [链接](https://youtu.be/pRYs49MqapI?si=PlKGMeGdJI7y3EdF)                        | 一系列解释核心开发和 Solana 概念的短视频                                                                                |
| Solana 课程                                | 教程      | freeCodeCamp  | [链接](https://web3.freecodecamp.org/solana)                                    | 旨在作为 Solana 开发介绍的引导式互动项目                                                                                   |
| Solana 教程                                | 视频        | Solana Foundation | [链接](https://www.youtube.com/@SolanaTutorials/videos)                         | 关于 Solana 和 Anchor 的综合视频                                                                                             |
| SolDev 的 Solana 开发课程                      | 教程      | Various       | [链接](https://www.soldev.app/course)                                           | 一个学习 Solana 开发的完整课程                                                                                             |
| Solana Cookbook                      | 文档 | Various       | [链接](https://solanacookbook.com/#contributing)                                | 一个开发者资源，提供在 Solana 上构建的基本概念和参考资料                             |

### Anchor 开发

| 标题                                                                     | 类型          | 作者(s)                       | 链接                                                                                                                     | 描述                                                                                                                                                                              |
|--------------------------------------------------------------------------|---------------|-------------------------------|--------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Anchor 简介：构建 Solana 程序的初学者指南                                 | 文章          | 0xIchigo                       | [链接](https://www.helius.dev/blog/an-introduction-to-anchor-a-beginners-guide-to-building-solana-programs)            | 学习您需要知道的一切，以开始使用 Anchor 在 Solana 上进行构建。                                                                                                             |
| Anchor                                                                    | 文档          | Coral                          | [链接](https://github.com/coral-xyz/anchor)                                                                            | Anchor 的官方文档，适用于 Solana 的 Sealevel 运行时框架。                                                                                                                  |
| 使用 React 和 Anchor 的全栈 Solana 开发                                   | 文章          | Solana 基金会                  | [链接](https://solana.com/developers/guides/getstarted/full-stack-solana-development)                                   | 逐步演示如何构建、测试和部署一个 Anchor 程序和 React 前端。                                                                                                               |
| 开始使用 Anchor 框架                                                   | 文章          | Solana 基金会                  | [链接](https://solana.com/developers/guides/getstarted/intro-to-anchor)                                                 | 介绍 Anchor，涵盖一个简单程序、IDL 和 TypeScript 客户端。                                                                                                                  |
| Anchor / Solana 开发简介                                                | 视频          | Harry Papacharissiou, Chainlink | [链接](https://www.youtube.com/live/Ru-ywR7rtgY?si=eLjKys3tkrehmKzJ)                                                    | 适合初学者的 Solana 和 Anchor 开发简介。                                                                                                                                   |
| Poseidon                                                                | 框架          | Turbin3                       | [链接](https://github.com/Turbin3/poseidon)                                                                             | 转换 Solana 程序的翻译器，将其从 TypeScript 转换为 Anchor。                                                                                                                |
| Solana 智能合约教程：使用 Anchor 框架                                    | 视频          | Josh's DevBox                 | [链接](https://youtu.be/CmG5_sIas1Q?si=oM19MuJB_x0pTV64)                                                              | 介绍 Anchor，属于 [“Solana 开发教程”系列](https://youtube.com/playlist?list=PL53JxaGwWUqCr3xm4qvqbgpJ4Xbs4lCs7&amp;amp;amp;amp;si=Kc1EqSTxlH8f7zob)。                       |
| Anchor 书籍                                                            | 文档          | Coral                          | [链接](https://book.anchor-lang.com/)                                                                                    | 一本入门书籍，帮助您开始学习 Anchor。                                                                                                                                      |

### 非 Anchor 程序开发

| 标题     | 类型      | 作者        | 链接                                           | 描述                                                               |
|-----------|-----------|-------------|------------------------------------------------|-------------------------------------------------------------------|
| Pinocchio | 框架      | Anza        | [链接](https://github.com/anza-xyz/pinocchio)  | 创建没有依赖项的 Solana 程序。                                     |
| Steel     | 框架      | Regolith Labs | [链接](https://github.com/regolith-labs/steel) | Solana 智能合约框架。                                            |

### 测试程序

| 标题                                  | 类型      | 作者(s)       | 链接                                                                  | 描述                                                                                                 |
|---------------------------------------|-----------|---------------|-----------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| Solana 程序测试指南                 | 文章      | 0xIchigo      | [链接](https://www.helius.dev/blog/a-guide-to-testing-solana-programs) | 了解如何测试 Solana 程序，从理论到实际示例。                                                       |
| Bankrun                               | 框架      | Kevin Heavey  | [链接](https://kevinheavey.github.io/solana-bankrun/)                 | 为 Solana 程序编写的轻量级、灵活的测试框架，使用 Node.js。                                         |
| LiteSVM                               | 框架      | LiteSVM 团队  | [链接](https://github.com/LiteSVM/litesvm)                            | 快速、轻量级的测试库，创建针对程序开发者优化的进程内 Solana 虚拟机。                             |
| Mollusk                               | 框架      | Joe Caulfield | [链接](https://github.com/buffalojoec/mollusk)                         | 小巧快速的 SVM 程序测试工具。                                                                       |
| solana-program-test                   | 框架      | Anza          | [链接](https://crates.io/crates/solana-program-test)                   | 一个基于 Rust 的测试框架，围绕 BanksClient 进行开发。                                             |
| solana-test-framework                 | 框架      | Halborn       | [链接](https://github.com/halbornteam/solana-test-framework)           | Halborn 开发的 **solana-program-test** 的扩展。                                                     |
| 使用 Anchor 进行测试                 | 视频      | Harry Papacharissiou, Chainlink | [链接](https://www.youtube.com/live/_9xS3ZvDIIU?si=YNJnfEMlGCKRFT6W)   | 在 Chainlink 2022 春季黑客马拉松中进行的关于测试 Anchor 程序的直播。                              |

### 程序安全

| 标题                                                      | 类型          | 作者(s)             | 链接                                                                                   | 描述                                                                                              |
|-----------------------------------------------------------|---------------|---------------------|----------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| Solana 程序安全的穿越指南                                 | 文章          | 0xIchigo, bl0ckpain | [链接](https://www.helius.dev/blog/a-hitchhikers-guide-to-solana-program-security)   | 了解 Solana 程序安全以及如何缓解常见漏洞。                                                        |
| Sealevel 攻击                                             | GitHub 仓库   | Coral               | [链接](https://github.com/coral-xyz/sealevel-attacks)                                 | 常见的针对 Solana 编程模型的攻击示例以及使用 Anchor 避免它们的推荐示例。                           |
| Solana 审计和安全资源                                     | GitHub 仓库   | 0xsanny             | [链接](https://github.com/0xsanny/solsec)                                             | 用于研究 Solana 智能合约安全、审计和漏洞的资源合集。                                            |
| Solana：审计师的入门介绍                                   | 文章          | OtterSec            | [链接](https://osec.io/blog/2022-03-14-solana-security-intro)                         | 关于 Solana 的安全性，探讨基础运行时环境、安全边界和影响的安全导论。                             |
| Solana 智能合约：常见陷阱及如何避免                      | 文章          | Neodyme             | [链接](https://neodyme.io/en/blog/solana_common_pitfalls/#intro)                     | 关于常见 Solana 安全陷阱及其缓解措施的简要介绍。                                                 |

### Crates 和 SDKs

| 标题              | 类型  | 作者(s) | 链接                                                         | 描述                                                               |
|-------------------|-------|---------|-------------------------------------------------------------|--------------------------------------------------------------------|
| helius            | Crate | Helius  | [链接](https://crates.io/crates/helius)                     | 一个异步 Helius Rust SDK，用于构建 Solana 的未来。                   |
| helius-sdk        | SDK   | Helius  | [链接](https://www.npmjs.com/package/helius-sdk/v/latest)   | 一个 Helius Node.js SDK，用于构建 Solana 的未来。                   |
| solana-program    | Crate | Anza    | [链接](https://crates.io/crates/solana-program)             | 所有 Solana 链上 Rust 程序的基础库。                               |
| solana-sdk        | Crate | Anza    | [链接](https://crates.io/crates/solana-sdk)                 | 官方 Solana SDK，用于用 Rust 编写客户端应用程序。                   |
| @solana/web3.js   | SDK   | Anza    | [链接](https://www.npmjs.com/package/@solana/web3.js/v/latest) | 一个为 Solana 构建的 JavaScript 客户端，基于 Solana JSON RPC API。 |

### 开发工具

| 标题                   | 类型      | 作者(s)             | 链接                                                                      | 描述                                                                                                                            |
|------------------------|-----------|---------------------|---------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
| Bubblegum              | 程序      | Metaplex            | [链接](https://github.com/metaplex-foundation/mpl-bubblegum)             | 创建和管理 Metaplex 压缩 NFT。                                                                                                 |
| Builderz dApp Scaffold  | 工具      | Builderz Labs       | [链接](https://github.com/builderz-labs/builderz-solana-dapp-scaffold)   | 一个开源的 Next.js Solana dApp 脚手架。                                                                                       |
| Builderz xNFT Scaffold  | 工具      | Builderz Labs       | [链接](https://github.com/builderz-labs/builderz-xNFT-scaffold-next)     | 一个开源的 Next.js Solana xNFT 背包脚手架。                                                                                     |
| cNFT 垃圾邮件过滤器      | 工具      | Solarnius           | [链接](https://github.com/filtoor/cnft-spam-filter)                      | 一个开源、轻量和可移植的 cNFT 垃圾邮件分类器。                                                                                  |
| create-solana-dapp      | 工具      | Solana 基金会       | [链接](https://github.com/solana-developers/create-solana-dapp)         | 创建 Solana dApps 的 CLI。                                                                                                     |
| Dreamcast              | 框架      | Joey Meere          | [链接](https://github.com/joeymeere/dreamcast)                          | 在几分钟内获取和交互 Anchor 程序。                                                                                           |
| Gill                   | 框架      | Solana 基金会       | [链接](https://github.com/solana-foundation/gill)                       | 用于与 Solana 区块链交互的 JavaScript/TypeScript 客户端库。                                                                  |
| Kite                   | 框架      | Helius              | [链接](https://github.com/helius-labs/kite)                             | 现代 TypeScript 框架，适用于 @solana/web3.js 2.0。                                                                        |
| Kinobi                 | 框架      | Metaplex            | [链接](https://github.com/metaplex-foundation/kinobi)                  | 为您的 Solana 程序生成强大的客户端。                                                                                           |
| Lighthouse             | 框架      | Jac0xb              | [链接](https://github.com/Jac0xb/lighthouse)                           | Solana 断言协议。                                                                                                            |
| Metaboss               | 工具      | Metafrost           | [链接](https://github.com/samuelvanderwaal/metaboss)                   | Metaplex NFT 标准的瑞士军刀工具。                                                                                              |
| PubKey Link            | 工具      | Beeman              | [链接](https://github.com/pubkeyapp/pubkey-link)                       | 基于 Solana 的免费开源 Discord 验证。                                                                                         |
| PubKey Stack           | 工具      | Beeman              | [链接](https://github.com/pubkeyapp/pubkey-stack)                      | 一个用于使用 PubKey 堆栈生成应用程序的起始工具。                                                                              |
| Shank                  | 框架      | Metaplex            | [链接](https://github.com/metaplex-foundation/shank)                   | 从 Solana Rust 合同中提取 IDL。                                                                                               |
| Skeet                  | 框架      | Skeet Dev           | [链接](https://github.com/elsoul/skeet)                                | 一个开源的 TypeScript 无服务器框架。                                                                                           |
| Solita                 | 框架      | Metaplex            | [链接](https://github.com/metaplex-foundation/solita)                  | Solana IDL 到 API 生成器。                                                                                                     |
| sol4k                  | 框架      | Sasha Shpota        | [链接](https://github.com/sol4k/sol4k)                                 | 用于 Solana 的 Kotlin 客户端，可与 Java 或任何其他 JVM 语言以及 Android 一起使用。                                             |
| Squads CLI             | 工具      | Squads              | [链接](https://github.com/Squads-Protocol/squads-cli)                  | 通过简单的 CLI 与 Squads 多签程序进行交互。                                                                                    |
| Turnkey Rust Client    | 框架      | Eliascm17           | [链接](https://github.com/Eliascm17/turnkey)                           | 与 Turnkey API 进行交互的 Rust 接口，允许通过安全 enclave 安全存储和签名交易。                                                  |
| Umi                    | 框架      | Metaplex            | [链接](https://github.com/metaplex-foundation/umi)                     | 用于 JavaScript 客户端的 Solana 框架。                                                                                         |
| Wallet Adapter         | 框架      | Anza                | [链接](https://github.com/anza-xyz/wallet-adapter)                     | 適用于 Solana 应用程序的模块化 TypeScript 钱包适配器及组件。                                                                  |

### 浏览器

| 标题              | 类型     | 作者(s)           | 链接                                   | 描述                                                            |
|-------------------|----------|-------------------|----------------------------------------|-----------------------------------------------------------------|
| SOL CLI Explorer   | 探索器   | cavemanloverboy   | [链接](https://github.com/cavemanloverboy/sol) | 一个用于 Solana 区块链的命令行探索器。                           |
| Solana Explorer    | 探索器   | Solana Labs       | [链接](https://explorer.solana.com/) | Solana 集群的官方探索器。                                       |
| SolanaFM           | 探索器   | SolanaFM 团队     | [链接](https://solana.fm/)           | 一个友好的 Solana 浏览器。                                      |
| Solscan            | 探索器   | Solscan 团队      | [链接](https://solscan.io/)          | 用户友好且实时扫描 Solana 生态系统的工具。                       |
| XRAY (旧版)       | 探索器   | Helius            | [链接](https://github.com/helius-labs/xray) | 由 Helius 提供的可读性强的 Solana 交易探索器。                    |

### 性能仪表板

| 标题                | 类型                                     | 作者(s)    | 链接                                                   | 描述                                                                |
|---------------------|------------------------------------------|------------|--------------------------------------------------------|---------------------------------------------------------------------|
| Chainstack Compare   | 节点性能监控仪表板                     | Chainstack | [链接](https://compare.chainstack.com/dashboard)       | 在时间上比较 Solana 节点的 RPC 性能仪表板，包括交易落地率。        |

### 游戏

| 标题                         | 类型        | 作者(s)                | 链接                                                                     | 描述                                                                                                                     |
|------------------------------|-------------|------------------------|--------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| Foundation Kit               | 框架        | Star Atlas             | [链接](https://github.com/staratlasmeta/FoundationKit)                   | 为虚幻引擎 4 和 5 创建的插件，允许虚幻游戏客户端连接和与 Solana 交互。                                             |
| GameShift                    | 框架        | Solana 实验室          | [链接](https://gameshift.solanalabs.com/)                                | 一个平台，方便游戏开发者通过单一 API 轻松集成 Web3 元素。                                                             |
| Godot SDK                    | 框架        | ZenRepublic, Virus-Axel | [链接](https://github.com/Virus-Axel/godot-solana-sdk)                  | 使 Godot 能够制作链上和 Solana 集成游戏的 GDExtension。                                                                |
| Honeycomb Protocol           | 框架        | Honeycomb Protocol 团队 | [链接](https://docs.honeycombprotocol.com/)                              | 为游戏开发者设计的一整套 Web3 工具。                                                                                    |
| MagicBlock                   | 游戏引擎    | MagicBlock 团队        | [链接](https://www.magicblock.gg/)                                       | 一款用于链上 SVM 游戏的多功能引擎。                                                                                     |
| Solana Unreal SDK            | 框架        | Bifrost Technologies    | [链接](https://github.com/Bifrost-Technologies/Solana-Unreal-SDK)      | 用于在 Solana 上使用虚幻引擎 5 构建区块链游戏的完整虚幻插件和工具包。                                                  |
| Solana Unity SDK             | 框架        | MagicBlock 团队        | [链接](https://docs.magicblock.gg/SolanaUnitySDK/overview)               | 一套全面的开源工具，方便在基于 Unity 的游戏中轻松访问 Solana。                                                       |
| Thugz BC Plugin Packaged     | 框架        | ThugzLabs              | [链接](https://github.com/ThugzLabs/Thugz-BC-Plugin-Packaged-for-UE5.0) | Thugz Labs BC 插件的打包版本，适用于虚幻引擎。                                                                          |
| Turbo                        | 游戏引擎    | Jozanza                | [链接](https://turbo.computer/)                                          | 特别为快速制作低分辨率、基于精灵的 2D 游戏而构建。                                                                    |

### 压缩

| 标题                                                                    | 类型          | 作者(s)                                               | 链接                                                                                                                             | 描述                                                                                                                        |
|-------------------------------------------------------------------------|---------------|-------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|
| 关于 Solana 状态压缩的所有知识                                           | 文章          | 0xIchigo                                              | [链接](https://www.helius.dev/blog/all-you-need-to-know-about-compression-on-solana)                                           | 了解状态压缩、压缩 NFT（cNFT）以及如何获取、铸造或转移它们。                                                              |
| 使用并发梅克尔树压缩数字资产                                           | 白皮书        | Jarry Xiao, Noah Gundotra, Austin Adams, Anatoly Yakovenko | [链接](https://drive.google.com/file/d/1BOpa5OFmara50fTvL0VIVYjtg-qzHCVc/view)                                              | 状态压缩背后的理论。                                                                                                     |
| 使用 JavaScript 创建压缩 NFT                                           | 文章          | Solana 基金会                                         | [链接](https://solana.com/developers/guides/javascript/compressed-nfts)                                                         | 创建树、铸造、读取和转移 cNFT 的逐步指南。                                                                                |
| 探索 Solana 上的 NFT 压缩                                               | 文章          | Mert Mumtaz                                           | [链接](https://www.helius.dev/blog/solana-nft-compression)                                                                      | 了解如何在 Solana 上处理 NFT 压缩。                                                                                       |
| 如何使用 TypeScript 铸造 Solana 压缩 NFT（cNFT）                         | 文章          | kishi.sol                                             | [链接](https://medium.com/@KishiTheMechanic/how-to-mint-solana-compressed-nfts-cnfts-with-typescript-be9d0fa7ce30)            | 使用 TypeScript 铸造 cNFT 的逐步指南。                                                                                    |
| 状态压缩                                                                | 文档         | Solana 基金会                                         | [链接](https://solana.com/docs/advanced/state-compression)                                                  | 状态压缩的官方文档。                                                                                                       |
| 状态压缩与压缩 NFT                                                          | GitHub 仓库   | solana-developers             | [链接](https://github.com/solana-developers/compressed-nfts)                                                                     | 使用压缩 NFT 的示例代码。                                                                                                  |
| 同时在 Solana 上铸造多个压缩 NFT (cNFT) 的小贴士                           | 文章          | kishi.sol                     | [链接](https://medium.com/@KishiTheMechanic/tips-for-minting-multiple-compressed-nfts-cnfts-simultaneously-on-solana-4e01e06bae00) | 同时铸造多个 cNFT 的小贴士。                                                                                              |
| ZK 压缩                                                                   | 文档          | Helius x Light Protocol       | [链接](https://www.zkcompression.com/)                                                                                           | 一种旨在减少状态成本几个数量级的新原语。                                                                                    |

### Solana 移动端

| 标题                                                | 类型          | 作者(s)                | 链接                                                                                          | 描述                                                                                                      |
|----------------------------------------------------|---------------|------------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
| 5 分钟内构建 cNFT 铸币移动应用                     | 文章          | Anam Ansari            | [链接](https://www.helius.dev/blog/build-a-cnft-minter-mobile-app-in-under-5-minutes)      | 涵盖如何构建 cNFT 铸造 Android 应用程序的教程。                                                           |
| iOS 上的密钥托管                                   | 文章          | Mike Sulistio          | [链接](https://docs.solanamobile.com/blog/ios-wallet-signing)                                  | 深入探讨 iOS 上密钥托管的模式和挑战。                                                                     |
| 移动 dApp 架构                                     | 文档          | Mike Sulistio          | [链接](https://docs.solanamobile.com/getting-started/mobile-dapp-architecture)                | 移动 dApp 架构概述，包括移动钱包适配器协议。                                                             |
| 发布 Solana 移动应用的指南                        | 文章          | 0xSolanaGirl           | [链接](https://www.helius.dev/blog/publishing-solana-mobile-apps)                             | 在 Solana 移动 dApp 商店发布的必要步骤和资源。                                                            |
| Solana 移动堆栈                                    | 文档          | Solana Mobile Team     | [链接](https://docs.solanamobile.com/)                                                        | 有关在 Solana 上进行移动开发的全面资源。                                                                   |
| Solana 移动教程应用                                | GitHub 仓库   | solana-mobile          | [链接](https://github.com/solana-mobile/tutorial-apps)                                       | 展示 Solana 移动堆栈（SMS）的教程应用程序集合。                                                            |
| Solana 的令牌门控 - Solana 移动教程                 | 文章          | 0xSolanaGirl           | [链接](https://www.helius.dev/blog/token-gating-on-solana-mobile-tutorial)                   | 学习如何使用 Saga Genesis Token 创建令牌门控体验。                                                        |

### Solana 支付

| 标题                                                | 类型          | 作者(s)                | 链接                                                              | 描述                                                                                                                |
|----------------------------------------------------|---------------|------------------------|-------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Shopify 和 Solana Pay：逐步指南（2023）               | 文章          | Owen Venter            | [链接](https://www.helius.dev/blog/solana-pay-shopify)            | 集成 Solana Pay 到 Shopify 商店的详细指南，涵盖商户设置和客户流程。                                               |
| Solana Pay                                         | GitHub 仓库   | Anza                   | [链接](https://github.com/anza-xyz/solana-pay)                    | 一种新的去中心化支付标准。                                                                                          |
| Solana Pay Android 示例                             | GitHub 仓库   | Solana Mobile Team     | [链接](https://github.com/solana-mobile/solana-pay-android-sample)| 针对 Android 钱包处理外部生成的 Solana Pay URI 的集成指南
| Solana Pay: 所有你需要知道的事情    | 文章          | Owen Venter       | [链接](https://www.helius.dev/blog/solana-pay)                     | Solana Pay 是一种标准协议和参考实现的集合，可以实现去中心化支付。                                       |
| 用100秒解释Solana Pay               | 视频          | Abdullah Raza     | [链接](https://youtu.be/nV6Y8nXS5-U?si=kMU8KVhs-1ONc21K)           | 一个有趣且简明扼要的解释，讲述了 Solana Pay 的工作原理、用途和优点。                                    |
| Solana Pay 规范                     | 文档          | Anza              | [链接](https://github.com/anza-xyz/solana-pay/blob/master/SPEC.md)   | Solana Pay 的规范文档。                                                                                  |

## 验证者

### Agave 客户端

| 标题                               | 类型          | 作者(s)         | 链接                                                                                                  | 描述                                                          |
|-------------------------------------|---------------|-----------------|---------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| Agave                               | GitHub 仓库   | Anza             | [链接](https://github.com/anza-xyz/agave)                                                               | Anza 的 Solana Labs 验证者客户端的分支。                      |
| Agave 过渡                          | 文档          | Anza             | [链接](https://github.com/anza-xyz/agave/wiki/Agave-Transition)                                        | Solana Labs 客户端迁移到新的 Agave 客户端的过程。           |
| Anza 的新 SVM API                   | 文章          | Joe Caulfield    | [链接](https://www.anza.xyz/blog/anzas-new-svm-api)                                                    | 定义 SVM 以及项目能够构建的内容。                             |
| Solana Labs 验证者客户端          | GitHub 仓库   | Solana Labs      | [链接](https://github.com/solana-labs/solana)                                                           | OG 验证者客户端。                                           |
| Agave 运行时                        | 文章          | Joe Caulfield    | [链接](https://fluff-ranunculus-275.notion.site/The-Agave-Runtime-d1f8d3608e5d4529b120e09e80b48887) | 深入探讨 Agave 运行时。                                   |

### Firedancer

| 标题                                                                                                                                  | 类型        | 作者(s)                    | 链接                                                                                                                                                                           | 描述                                                                                                                           |
|----------------------------------------------------------------------------------------------------------------------------------------|-------------|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Breakpoint 2023: Firedancer 更新                                                                                                     | 视频       | Dan Albert                   | [链接](https://youtu.be/hEEWMiMuEF8?si=tiW4lJFisBAOgwXb)                                                                                                                       | Dan Albert 在 Breakpoint 2023 上介绍的 Firedancer 更新。                                                                         |
| Breakpoint 2023: FPGA 以 8M TPS 工作                                                                                                   | 视频       | Kaveh Aasaraai, Kevin Bowers | [链接](https://youtu.be/1oQg2_b_gv8?si=G5VE8g4UAu-AE6Zw)                                                                                                                       | 在 Breakpoint 2023 上的演讲，演示 Firedancer 如何在一台 8 年旧的机器上，以 7 年旧的 FPGA 实现 800 万 TPS。                    |
| Breakpoint 2023: 网络通信的快速 Reed-Solomon 编码                                                                                     | 视频       | Philip Taffet                | [链接](https://youtu.be/rXB8NO15Mv4?si=XI4f5VtMaEHfd2w5)                                                                                                                       | 在 Breakpoint 2023 的演讲，讲述 Firedancer 如何优化 Reed-Solomon 编码以用于其网络通信。                                     |
| Breakpoint 2023: Securing Firedancer                                                                                                   | 视频       | Felix Willhelm               | [链接](https://youtu.be/K6H1TRbiaR4?si=U8P904PT7oFlI8Eb)                                                                                                                       | 在 Breakpoint 2023 的演讲，讨论 Firedancer 的安全考虑和实现。                                                                 |
| Firedancer                                                                                                                             | GitHub 仓库 | Firedancer 团队              | [链接](https://github.com/firedancer-io/firedancer)                                                                                                                            | Firedancer 是 Jump Crypto 的 Solana 共识节点                                                                              |
| Firedancer 可靠性努力                                                                                                                   | 文章       | Richard Patel                | [链接](https://jumpcrypto.com/writing/firedancer-reliability/)                                                                                                                 | 本文介绍了 Firedancer 如何提高 Solana 的吞吐量和可靠性                                                   |
| Firedancer 的 fd_quic 技术里程碑                                                                                                  | 主题      | Firedancer 团队              | [链接](https://x.com/jump_firedancer/status/1654124396062158850)                                                                                                   | 一个关于 Firedancer 高性能实现 QUIC 和 Solana 吸收网络协议的 Twitter 线程                                     |
| Jump Crypto 着手构建新的验证者客户端，以提高 Solana 区块链的吞吐量和可靠性                                                       | 文章      | Kevin J Bowers               | [链接](https://jumpcrypto.com/writing/jump-crypto-sets-out-to-build-new-validator-client-for-the-solana-blockchain-to-increase-the-throughput-and-reliability-of-the-network/) | Jump Crypto 的 Firedancer 宣告                                                                                                          |
| 跳跃与光速的比较                                                                                                                  | 文章      | Kevin J Bowers               | [链接](https://jumpcrypto.com/writing/jump-vs-the-speed-of-light/)                                                                                                       | “光速太慢了”                                                                                                                                |
| Firedancer 是什么？深入了解 Solana 2.0                                                                                             | 文章      | 0xIchigo                     | [链接](https://www.helius.dev/blog/what-is-firedancer)                                                                                                                   | 了解关于 Firedancer 的所有信息，这是 Jump 开发的 Solana 新独立验证者客户端                                         |

### 更新

| 标题                                              | 类型    | 作者       | 链接                                                                                         | 描述                                                                                                                              |
|--------------------------------------------------|---------|------------|----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| 关于 Solana 的 v1.16 更新你需要知道的一切       | 文章    | 0xIchigo   | [链接](https://www.helius.dev/blog/all-you-need-to-know-about-solanas-v1-16-update)         | 了解 Solana 的 v1.16 更新，这是 Solana Labs 验证者客户端的最新升级                                                             |
| 关于 Solana 的 v1.17 更新你需要知道的一切       | 文章    | 0xIchigo   | [链接](https://www.helius.dev/blog/all-you-need-to-know-about-solanas-v1-17-update)         | 了解 Solana 的 v1.17 更新，这是 Solana Labs 验证者客户端的最新升级，以及最近的二月份网络故障                                     |
| 关于 Solana 的 v1.18 更新你需要知道的一切       | 文章    | 0xIchigo   | [链接](https://www.helius.dev/blog/all-you-need-to-know-about-solanas-v1-18-update)         | 了解关于 Solana Labs（现为 Agave）客户端的最新更新，以及新的中央调度程序                                                      |
| Agave v2.0 更新你需要知道的一切                  | 文章    | Lostin     | [链接](https://www.helius.dev/blog/agave-v2-update)                                         | 总结了 Solana Agave 2.0 的关键特性和优化，包括系统调用、经济变化和 ZK ElGamal 证明                                          |
| Agave v2.1 更新：你需要知道的一切                 | 文章    | Lostin     | [链接](https://www.helius.dev/blog/agave-v21-update-all-you-need-to-know)                  | 总结了 Solana Agave 2.1 客户端更新中需要关注的所有主要发布周期特性和优化                                                      |

### 结构

| 标题                                                                | 类型    | 作者                | 链接                                                                                                     | 描述                                                                                                                                                     |
|-------------------------------------------------------------------|---------|--------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| 介绍中央调度器：Agave v1.18 的可选功能                           | 文章    | Rex St. John       | [链接](https://www.anza.xyz/blog/introducing-the-central-scheduler-an-optional-feature-of-agave-v1-18) | 介绍 Agave v1.18 更新中的新中央调度器                                                                                                 |
| 关于 Solana 9 月 14 日故障的反思                                   | 文章    | Jump Crypto        | [链接](https://jumpcrypto.com/writing/reflections-on-the-sept-14-solana-outage/)                       | 对早期 Solana 故障事件的深入分析                                                                                                      |
| Solana 银行阶段和调度器                                          | 文章    | Andrew Fitzgerald  | [链接](https://apfitzge.github.io/posts/solana-scheduler/)                                             | 深入解释 Solana Labs 验证器客户端在块生产中使用的历史、当前和即将到来的调度算法和设计                                                    |
| 从基本原理看 Solana 的发行                                        | 文章    | Matt Resnick        | [链接](https://www.anza.xyz/blog/solana-issuance-from-first-principles)                                 | 从根本上了解 Solana 的发行及当前的发行是否最优                                                                 |
| 聚焦：Solana 的调度器                                            | 视频    | Solana Foundation  | [链接](https://youtu.be/R7hq8ampBio?si=oCLdEVJs46clJ2gv)                                               | 对 1.17 版调度器的关键分析，交易如何通过银行阶段，以及未来 1.18 版调度器的工作原理                                                                             |
| Solana eBPF 虚拟机                                               | 文章    | Joe Caulfield       | [链接](https://www.anza.xyz/blog/the-solana-ebpf-virtual-machine)                                        | 了解 rBPF 虚拟机的工作原理，以及验证者如何使用它执行程序                                                                                              |
| Solana 验证者 101：交易处理                                      | 文章    | Jito Labs          | [链接](https://www.jito.wtf/blog/solana-validator-101-transaction-processing/)                         | 对交易生命周期的技术深入探讨                                                                                                           |

### 运营、维护与经济学

| 标题                                        | 类型          | 作者(s)            | 链接                                                                         | 描述                                                                    |
|----------------------------------------------|---------------|----------------------|------------------------------------------------------------------------------|---------------------------------------------------------------------------|
| 如何设置 Solana 验证者                       | 文章          | John Sloboda         | [链接](https://www.helius.dev/blog/how-to-set-up-a-solana-validator)         | 学习如何启动和运行 Solana 主网验证者                                     |
| 运行 Solana 验证者：全面解析                 | 文章          | Fikunmi Ajayi-Peters | [链接](https://apfikunmi.medium.com/running-a-solana-validator-a95cdfd6488a) | 关于验证者、运行一个的经济学与盈利能力的全面指南                       |
| 设置 Solana 验证者                           | 文档          | Solana Foundation    | [链接](https://docs.solanalabs.com/operations/setup-a-validator)             | Solana 官方文档，关于运行验证者的信息                                   |
| 从第一原则看 Solana 的发行                   | 文章          | Max Resnick          | [链接](https://www.anza.xyz/blog/solana-issuance-from-first-principles)       | 学习 Solana 的发行方式及当前发行是否最优                               |
| Solana 验证者经济学：入门                     | 文章          | Ryan Chern           | [链接](https://www.helius.dev/blog/solana-validator-economics-a-primer)      | Solana 验证者经济学的入门指南                                         |
| Solana 验证者运营最佳实践                     | 文档          | Solana Foundation    | [链接](https://docs.solanalabs.com/operations/best-practices/general)        | Solana 官方文档推荐的最佳实践                                         |
| 验证者利润计算器                             | 工具          | Cogent Crypto        | [链接](https://cogentcrypto.io/ValidatorProfitCalculator)                    | 用于估计验证者在假设场景下的收益的工具                                 |

### 观点和文章

| 标题                                                            | 类型    | 作者(s)                                   | 链接                                                                                                                                                                      | 描述                                                                                                                                        |
|------------------------------------------------------------------|---------|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| 超越技术男：重新思考加密领域中的偶像崇拜                      | 文章 | 0xIchigo                                    | [链接](https://www.helius.dev/blog/beyond-the-tech-bro-rethinking-hero-worship-in-crypto)                                                                                  | 个人崇拜、大人物的历史理论、思想的力量、去中心化领导、草根组织、加密乐观主义。                                                            |
| 狗币、猫视频和颠覆                                            | 文章 | Mikel Ayala                                 | [链接](https://medium.datadriveninvestor.com/dog-coins-cat-videos-and-disruption-79cfa4ff69c0)                                                                            | 对 meme 币、注意力经济、在线社区和数字原生资本的批判性分析                                                                               |
| 铸造去中心化的知识——每个革命都需要一个火花                  | 文章 | M3taversal                                  | [链接](https://medium.com/@m3taversal/forging-decentralized-knowledge-every-revolution-needs-a-spark-59b8c80c1db6)                                                        | 对一项变革性 Web3 项目的本质进行批判性分析，旨在创建一个经得起时间考验的知识库。                                                         |
| Solana：如何颠覆区块链                                        | 文章 | Lee Nguyen                                  | [链接](https://open.substack.com/pub/stationoneohone/p/solana-how-it-revolutionized-blockchain?r=3hghbx&amp;amp;amp;amp;utm_campaign=post&amp;amp;amp;amp;utm_medium=web) | 从创始到未来的 Solana 故事。                                                                                                               |
| Solana 夏季                                               | 文章 | Packy McCormick                             | [链接](https://www.notboring.co/p/solana-summer)                                                                                                                          | 关于 Solana 故事的全面而引人入胜的阅读。                                                                                                   |
| SOL 生存者                                                  | 文章 | 0xsmac                                      | [链接](https://0xsmac.substack.com/p/sol-survivor)                                                                                                                        | 关于 Solana 成为一个引人注目的资产和网络的独特视角。                                                                                     |
| 几亿用户之路                                                | 文章 | James Carlin                                | [链接](https://clean-winter-ede.notion.site/The-Billion-User-Path-5310014e09cb49bc83e9ee099ca12c7f)                                                                        | 对区块链的未来以及用户破十亿用户的乐观分析                                                                                             |
| Helius 宣言                                      | 宣言        | Mert Mumtaz                | [链接](https://www.helius.dev/blog/manifesto)                                                                               | Helius 的使命是提高全球开发者的经济潜力。我们相信，这只有通过加密基础设施才能实现。                                                |
| Solana 繁荣的那一年                              | 文章        | Ryan Shea                  | [链接](https://writing.ry.sh/the-year-solana-blew-up-6d50cccb4615)                                                         | 对于任何对 Solana 感兴趣的人来说，这是一篇必读的文章。                                                                        |
| 为什么选择 Solana                                 | 文章        | Mert Mumtaz                | [链接](https://www.mertimus.com/p/why-solana)                                                                               | 关于在 Solana 上构建的个人观点。                                                                                              |
| Solana 论点 - 最快的马是如何从灰烬中崛起的        | 文章        | Ryan Watkins, Wilson Withiam, Daniel Cheung | [链接](https://www.syncracy.io/writing/solana-thesis)                                                                        | 一篇全面的论文，解释 Solana 的“为什么”。                                                                                     |

## Solana 的未来

| 标题                                           | 类型        | 作者(s)                | 链接                                                         | 描述                                                                                                                       |
|------------------------------------------------|-------------|------------------------|--------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| Solana 中的异步程序执行 (APE)                  | 文章        | Anatoly Yakovenko      | [链接](https://x.com/aeyakovenko/status/1804937522998591577) | 一篇推特文章，讨论异步执行以及独立于其他程序运行投票程序的目标。                                                            |
| Solana 上的状态增长问题                        | 文章        | Anatoly Yakovenko      | [链接](https://x.com/aeyakovenko/status/1796569211273445619) | 一篇推特文章，讨论 Solana 状态的快速增长及其潜在解决方案。                                                                  |

