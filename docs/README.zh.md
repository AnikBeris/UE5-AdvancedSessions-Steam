<p align="center">
  <strong>-------></strong>
  <a href="/README.md">俄语</a> |
  <a href="/docs/README.en.md">英语</a> |
  <a href="/docs/README.es.md">西班牙语</a> |
  <a href="/docs/README.zh.md">中文</a> |
  <strong><-------</strong>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../media/logo-dark.png">
    <img alt="项目Logo" src="../media/logo-light.png" width="512" height="auto">
  </picture>
</p>

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-blue?style=flat&logo=github)](https://github.com/AnikBeris)
[![License](https://img.shields.io/badge/License-purple?style=flat&logo=github)](/LICENSE.md)
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=星星&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="分隔符" width="90%">
</div>


<h1 align="center"> 
在使用AdvancedSessions-Steam插件时，关于Unreal Engine 5项目开发的有用信息
</h1>

<h2 align="center">
> 💡 本材料面向有经验的用户。
</h2>

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
⚠️ 免责声明 ⚠️
</h2>

<p align="center">
  作者不对使用本项目可能产生的任何后果承担责任。<br>
  使用者需自担风险使用。
</p>

<details align="center"> 
    <summary>⚠️全文⚠️</summary>

使用此存储库中的内容需自担风险。

1. 使用此存储库内容，即表示您自动同意与之相关的许可协议条款。

2. 作者对这些材料的准确性、完整性或适用性不作任何明示或默示的保证。

3. 作者不对由于使用或无法使用本存储库中的材料或其附带文档而导致的任何损失负责，包括但不限于直接、间接、附带、间接或特别损失，即使事先已告知有可能造成此类损失。

4. 使用本存储库内容即表示您确认并接受所有相关风险。此外，您同意作者对因使用本项目而产生的任何问题或后果不负任何责任。

</details> 

---

<h3 align="center"> 
💖 支持本项目 
</h3>

<p align="center"> 
如果本项目对您有帮助，您可以通过点亮一颗小星星来支持我们。:star2: 
</p>

<p align="center">
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="请我喝杯咖啡">
  </a>
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="请我喝杯咖啡">
  </a>
</p>

<h4 align="center"> 
小额捐赠深受欢迎，无论金额多少，我们都非常感谢。😌 
</h4>

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
  <sub> 感谢您关注和支持本项目 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

## 📚 目录

- [简介](#-简介)

## 🔗 有用链接

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
  <a href="#-目录"> ⬆️ 返回顶部 </a> 
</h2>

<h1 align="center"> 
技术要求
</h1>

## 📊 已安装插件

<details> 
    <summary>⚙️ 展开描述</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 

## 📊 禁用插件

<details> 
    <summary>⚙️ 展开描述</summary>

- **SteamSockets:** SteamSockets插件驱动程序用于Steam的工作，但在使用Advanced Sessions Plugin的情况下需要禁用它。

</details> 

## 📊 功能 || 特性

<details> 
    <summary>⚙️ 展开描述</summary>

</details>

<h2 align="center">
  <a href="#-目录">⬆️ 返回顶部</a> 
</h2>

###### # 项目 - 地图与模式

<h1 align="center"> 
项目 - 地图与模式 
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## 此章节目的

**项目 - 地图与模式**章节定义了游戏流程和项目架构的关键入口点，它设置了以下内容：

---

- 使用的默认`GameMode`；
- 启动编辑器、游戏和服务器时加载的地图；
- 应用的基本类（`Pawn`，`Controller`，`HUD`等）；
- 根据地图或地图前缀自动替换`GameMode`。

这实际上是**游戏流程架构中的入口点**。

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

...

完整中文翻译内容，请继续扩展或提供您需要更多内容部分。
