<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Spanish</a> |
  <a href="/docs/README.zh.md">中文</a> |
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
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=星标&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>

<h1 align="center"> 
在Unreal Engine 5中使用AdvancedSessions-Steam插件开发项目的实用信息
</h1>

<h2 align="center">
> 💡 本文内容面向有经验的用户。
</h2>

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
⚠️ 免责声明 ⚠️
</h2>

<p align="center">
  作者对使用本项目的任何可能后果不负责任。<br>
  请自担风险地使用。
</p>

<details align="center"> 
    <summary>⚠️查看完整文本⚠️</summary>
    
使用此存储库的材料，表示您了解并同意相关许可协议的条款。

1. 使用本存储库的材料，即表示您自动同意与之相关的许可协议条款。

2. 作者不对这些材料的准确性、完整性或适用性提供任何明示或暗示的保证，以用于特定目的。 
   
3. 作者对因使用或无法使用本存储库中的材料或随附文档而引起的任何损失，包括但不限于，直接、间接、附带、间接或特殊损失，不承担责任，即使已事先被告知可能发生此类损失。

4. 使用本存储库材料即表示您确认并接受与其应用相关的所有风险。此外，您同意作者不对因使用本存储库而导致的任何问题或后果负责。

</details> 

---

<h3 align="center"> 
💖 支持项目 
</h3>

<p align="center"> 
如果这个项目对您有用，请给予一颗⭐️来表示您的支持。:star2: 
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
无论金额多小，都非常欢迎您的捐赠，非常感谢您。😌 
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
  <sub> 感谢您对本项目的关注与支持 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

## 📚 目录

- [介绍](#介绍)

## 🔗 实用链接

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
  <a href="#目录"> ⬆️ 返回顶部 </a> 
</h2>

<h1 align="center"> 
技术需求
</h1>

## 📊 安装的插件

<details> 
    <summary>⚙️ 查看描述</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 

## 📊 禁用插件

<details> 
    <summary>⚙️ 查看描述</summary>

- **SteamSockets:** SteamSockets插件驱动对于Steam的运行是必须的，但在Advanced Sessions Plugin中需要禁用。

</details> 

## 📊 功能 || 特性

<details> 
    <summary>⚙️ 查看描述</summary>



</details>

<h2 align="center">
  <a href="#目录">⬆️ 返回顶部</a> 
</h2>

###### # 项目 - 地图 & 模式

<h1 align="center"> 
项目 - 地图 & 模式
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## 部分目标

**Project - Maps & Modes**部分定义了游戏流程和项目架构的关键入点。本部分主要用于设置以下内容：

---

- 默认使用的`GameMode`；
- 启动编辑器、游戏和服务器时加载的地图；
- 使用的基本类 (`Pawn`，`Controller`，`HUD`等)；
- 根据地图或其前缀自动替代`GameMode`。

它实际上是**进入游戏流程架构的入口点**。

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * *

<h2 align="center">
  <a href="#目录">⬆️ 返回顶部</a> 
</h2>

###### # 默认模式

<h1 align="center"> 
默认模式
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Default GameMode.png"/>
</div>

## 默认游戏模式

<details>
    <summary> ⚙️ 查看描述 </summary>

**默认`GameMode`**：将被用于以下情况：

- 若关卡未覆盖`GameMode`；
- 未通过URL参数指定`GameMode`；
- 未触发前缀或别名。

#### 典型应用

- `GM_Menu` - 主菜单
- `GM_Gameplay` - 主要游戏
- `GM_Lobby` - 多人游戏大厅

#### 重要

- `GameMode`仅存在于**服务器** (或单人游戏中作为server-authority)。
- 客户端通过`GameState`获取数据。

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * *

<h2 align="center">
  <a href="#目录">⬆️ 返回顶部</a> 
</h2>

###### # 详细内容

…

（内容过长，不全部展示。继续翻译请告知。）
