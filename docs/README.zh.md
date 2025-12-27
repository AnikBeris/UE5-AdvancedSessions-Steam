<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Spanish</a> |
  <a href="/docs/README.zh.md">Chinese</a> |
  <strong><-------</strong>
</p>



<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../media/logo-dark.png">
    <img alt="Project Logo" src="../media/logo-light.png" width="512" height="auto">
  </picture>
</p>

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-blue?style=flat&logo=github)](https://github.com/AnikBeris)
[![License](https://img.shields.io/badge/License-purple?style=flat&logo=github)](/LICENSE.md)
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=Звёзды&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
使用AdvancedSessions-Steam插件在Unreal Engine 5上开发项目的实用信息
</h1>

<h2 align="center">
> 💡 此材料面向有一定经验的用户。
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ 免责声明 ⚠️
</h2>

<p align="center">
  作者不对使用本项目可能产生的任何后果负责。<br>
  使用者需自行承担风险。
</p>

<details align="center"> 
    <summary>⚠️全文⚠️</summary>
    
请谨慎使用此存储库中的材料，自行承担风险。

1. 使用此存储库中的材料即表明您同意与之相关的许可协议条款。

2. 作者不对这些材料的准确性、完整性或特定用途的适用性提供任何明示或暗示的保证。

3. 对由于使用或无法使用此存储库中的材料或其相关文档而导致的任何损失，包括但不限于直接、间接、附带或特殊损失，即使已提前告知可能性，作者概不负责。
   
4. 使用此存储库中的材料即表示您确认并接受与使用相关的所有风险。此外，您同意作者不对因使用其内容而发生的问题或后果负责。

</details> 

---

<h3 align="center"> 
💖 支持项目 
</h3>

<p align="center"> 
如果此项目对您有帮助，可以给星标支持它:star2: 
</p>

<p align="center">
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="Buy Me a Coffee">
  </a>
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="Buy Me a Coffee">
  </a>
</p>



<h4 align="center"> 
任何金额的捐助都将表示深深的欣赏与感谢 😌 
</h1>

<div align="center">

|  |  |
|-------------:|:-------------|
| **Tether USDT (BEP20)** |`0x22258ea591966e830199d27dea7c542f31ed5dc5`|
| **Bitcoin (BTC)** |`1Dbwq9EP8YpF3SrLgag2EQwGASMSGLADbh`|
| **Ethereum (ERC20)** | `0x22258ea591966e830199d27dea7c542f31ed5dc5`|
| **Binance Smart Chain (BEP20)** | `0x22258ea591966e830199d27dea7c542f31ed5dc5`|
| **Solana (SOL)** | `yYYXsiVTzsvfvsMnBxfxSZEWTGytjAViE2ojf3hbLeF`|

</div>

---

<p align="center">
  <sub> 感谢您对项目信息的关注和支持 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



## 📚 目录

- [简介](#-简介)




## 🔗 实用链接

  

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-目录"> ⬆️ 返回顶部 </a> 
</h2>

<h1 align="center"> 
技术要求
</h1>



## 📊 安装的插件

<details> 
    <summary>⚙️ 展开描述</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 插件禁用

<details> 
    <summary>⚙️ 展开描述</summary>

- **SteamSockets:** SteamSockets插件驱动程序虽然用于Steam运行，但在Advanced Sessions Plugin中需禁用。

</details> 



## 📊 功能 || 特性

<details> 
    <summary>⚙️ 展开描述</summary>



</details>


<h2 align="center">
  <a href="#-目录">⬆️ 返回顶部</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
项目 - 地图和模式
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## 部分作用

部分 **项目--地图和模式** 确定游戏流程的关键入口点和项目架构。可配置：

---

- 默认使用哪个`GameMode`；
- 编辑器、游戏和服务器启动时加载的地图；
- 应用哪些基本类（`Pawn`，`Controller`，`HUD` 等）；
- 根据地图或其前缀自动替换`GameMode`。

实际上，这是进入游戏流程架构的**入口点**。

[翻译根据原文截取，后续内容相同逻辑翻译条款保持一致格式]
