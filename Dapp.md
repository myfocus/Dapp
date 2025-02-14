# 0. 讲师简介

自媒体「Keegan小钢」

# 1. 什么是 Web3

## Web3 == Web3.0?

Web3 (also known as Web 3.0) - by [Wikipedia](https://en.wikipedia.org/wiki/Web3)
[Decentralized Web and Semantic Web](https://www.nexxworks.com/blog/web3-and-web-3-0-are-not-the-same-thing-heres-why)

## 定义

目前没有标准的定义，但普遍认为：

- Web1 是只读的，Web2 是读+写，Web3 是读+写+拥有。
- Web3 是一个利用区块链技术实现无信任、无许可和去中心化的价值网络。

核心在于理解「拥有」两字，拥有的本质是「所有权」，而所有权的载体主要是通过 Token 体现，所以 Web3 的核心不能没有 Tokenomics。

## 登录方式的对比

![](./images/Web1,2,3-login.png)

## 内容交互的对比

![](./images/Web1,2,3-content.png)

# 2. Web3 的组成架构

![](./images/web3-layers.png)

## 协议层

即底层区块链架构层，包括 **Layer1** 的各种区块链，也包括 **Layer2** 的各种扩展链，还包括**跨链桥**。

- **Layer1**：Ethereum、BSC、Heco、Avalanche、Near、Solana、Cosmos、Polkadot、Aptos、Sui
- **Layer2**：Optimism、Arbitrum、zkSync、StarkNet
- **Bridge**：Synapse、Hop、AnySwap

## 基础设施层

由一些可互操作的构建模块组成，是一个比较多样化的一层，以下列出的只是部分模块：

- **链上金融协议**：Uniswap、Curve、Compound、Aave
- **数据存储**：IPFS、Arweave
- **数据分析**：Chainalysis、Covalent、Dune Analytics
- **合约安全**：Certik、OpenZeppelin
- **通信协议**：XMTP、matrix、swarm
- **用户身份**：ENS
- **预言机**：Chainlink
- **数据索引服务**：Graph

## 应用层

与用户交互的应用层，有着各种不同类型的应用，如游戏、内容、NFT、金融服务等。

- **游戏**：Axie Infinity、illuvium、Decentraland
- **内容**：Mirror、rally、Context
- **NFT**：OpenSea、Rarible、Mintbase
- **金融服务**：Uniswap、Matcha

**注意**：这里又出现了 **Uniswap**。可以思考下为什么？

## 访问层

即访问 Web3 的入口，包括钱包、浏览器等，还有一些聚合器，甚至一些 Web2 平台也成为了 Web3 的入口。

- **钱包**：MetaMask、Dipperex Token、Ledger、Terzor、Gnosis Safe、Moonbeam Safe
- **浏览器**：Brave
- **聚合器**：DappRadar、DeBank、Zerion
- **Web2**：twitter、reddit、discord

# 3. Web3 的现状与趋势

## 搜索热度

[全球搜索热度](https://trends.google.com/trends/explore?date=today%205-y&q=web3)

## 各赛道现状与趋势

[我眼中区块链各个赛道正在演进的技术趋势](https://mirror.xyz/0x2C4B9083c95F7c33d78B6088979fCE9B2c493Fe6/dj3qXEGWF5qpJkeV2Yygc9-VPiGiAo8UQCOIq6fJfYc)
![](./images/web3各赛道现状与趋势.jpeg)

## DApp 统计数据

https://www.stateofthedapps.com/stats

## 找 Web3 工作的渠道

- [web3.career](https://web3.career/)
- [cryptocurrencyjobs.co](https://cryptocurrencyjobs.co/)
- [remote3.co](https://remote3.co/)
- [Linkedin](https://www.linkedin.com/jobs/)
- [Rebase 社区](https://mp.weixin.qq.com/mp/appmsgalbum?action=getalbum&__biz=MzU0ODk1MTE1MA==&scene=1&album_id=1644470749073555457&count=3#wechat_redirect)
- **内推**

## 总结

- EVM 系已经形成庞大的生态基础，其地位已经难以撼动
- EVM 系的应用层存在更多发展机会
- 基于 Solidity 的 Dapp 人才需求庞大

# 4. Dapp 的技术架构

## 整体架构

![](./images/Dappjiagou.png)

- **Blockchain**：底层的区块链网络，一个 DeFi 应用一般都会部署到多个不同的区块链网络
- **Smart Contracts**：智能合约，是 DeFi 应用的核心业务实现，也是灵魂所在
- **Price Oracle**：价格预言机，用来提供价格信息的，一般可分为链下预言机和链上预言机
- **Keeper Services**：智能合约的任务触发器和执行器，因为智能合约本身没有自动触发执行任务的能力，所以需要外部的任务触发器协助
- **Subgraph**：子图，也被称为索引器，主要将链上数据重新组装成方便前端查询的数据
- **Graph Node**：Subgraph 所运行的环境，会同步链上区块数据给 Subgraph 处理
- **Wallet**：钱包应用，最主流的就是 MetaMask
- **WebUI**：前端展示的 UI 页面，一般用 Vue、React 等前端框架
- **SDK**：封装了对 Subgraph 的查询、智能合约的调用、钱包的连接等，方便前端 UI 的调用

## 技术栈和开发工具

- Solidity
- Rust/Golang
- Visual Studio Code
- Remix
- Hardhat/Truffle
- Graph & Subgraph
- Ethers.js/Web3.js
- MetaMask
- Infura/Alchemy
- Tenderly
