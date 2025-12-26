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
    <img alt="项目徽标" src="../media/logo-light.png" width="512" height="auto">
  </picture>
</p>

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-blue?style=flat&logo=github)](https://github.com/AnikBeris)
[![License](https://img.shields.io/badge/License-purple?style=flat&logo=github)](/LICENSE.md)
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=Star&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
在使用AdvancedSessions-Steam插件的情况下开发Unreal Engine 5项目的实用信息
</h1>

<h2 align="center">
> 💡 该材料针对有一定开发经验的用户。
</h2>

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
⚠️ 免责声明 ⚠️
</h2>

<p align="center">
  作者对于使用该项目可能产生的任何后果概不负责。<br>
  使用请自行承担风险。
</p>

<details align="center"> 
    <summary>⚠️完整文本⚠️</summary>
    
使用本库中的材料请自行承担风险。

1. 使用本库中的资料即代表您自动同意与之相关的许可协议条款。

2. 作者不对这些材料的准确性、完整性或适用于任何特定目的的明确或隐含保证负责。

3. 作者不对因使用或无法使用本库中的资料或相关文档而引起的任何损失负责，包括但不限于直接、间接、附带、后果性或特殊的损失，即使已提前告知可能存在该类损失的可能性。

4. 使用本库材料，您确认并接受所有风险。同时，您同意作者对其使用所引发的任何问题或后果不承担任何责任。

</details> 

---

<h3 align="center"> 
💖 支持本项目 
</h3>

<p align="center"> 
如果本项目对您有所帮助，欢迎为本项目点赞收藏。:star2: 
</p>

<p align="center">
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="请我喝咖啡">
  </a>
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="请我喝咖啡">
  </a>
</p>

<h4 align="center"> 
哪怕是微小的捐赠也将备受欢迎，非常感谢您的支持。😌 
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
  <sub> 感谢您对本项目的关注和支持 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

## 📚 目录

- [简介](#-简介)

## 🔗 有用的链接

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
  <a href="#-目录"> ⬆️ 回到顶部 </a> 
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

## 📊 禁用插件

<details> 
    <summary>⚙️ 展开描述</summary>

- **SteamSockets:** `SteamSockets` 插件驱动是 Steam 服务所需，但在使用 Advanced Sessions Plugin 时需要禁用。

</details> 

## 📊 功能 || 特点

<details> 
    <summary>⚙️ 展开描述</summary>

</details>

# 项目 - 地图与模式

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## 此部分目的

**Project - Maps & Modes** 定义了游戏流程和项目架构中的关键入口点。它可以设置：

---

- 默认使用的 `GameMode`；
- 编辑器、游戏和服务器启动时加载的地图；
- 应用的基本类（`Pawn`、`Controller`、`HUD` 等）；
- 如何根据地图或其前缀自动替换 `GameMode`。

这实际上是**游戏流程架构的入口点**。

---

# 默认模式

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Default GameMode.png"/>
</div>

## 默认 GameMode

**默认 GameMode** 是：

- 当地图未覆盖 `GameMode` 时使用；
- 未通过 URL 参数指定 `GameMode`；
- 前缀或别名未生效时。

#### 典型用途

- `GM_Menu` - 主菜单
- `GM_Gameplay` - 核心游戏
- `GM_Lobby` - 多人大厅

#### 重要

- `GameMode` **仅存在于服务器上**（或单人模式中作为服务器权限存在）。
- 客户端通过 `GameState` 获取数据。

---

## 已选择的 GameMode

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

该部分为选定的 `GameMode`（此处为 `GM_Menu`）定义类集合。

---

### 默认 Pawn 类

指定将为玩家自动生成的 `Pawn`。

示例：

- `Pawn` - 用于菜单的简单空对象
- `Character` - 完整角色
- `SpectatorPawn` - 用于观察模式

对于菜单：

- 通常使用空 `Pawn` 或具有简单逻辑且无操作控制。

---

### HUD 类

`HUD` 类（尽管已过时，仍受支持）。

用途：

- 如果通过 `DrawHUD` 绘制 UI；
- 旧 HUD 逻辑。

现代做法：

- `HUD` 为空；
- 在 `PlayerController` 中通过 **UMG** 创建 UI。

在菜单中使用 `HUD_Menu` 是可以接受的。

---

### 玩家控制器类

架构中的关键类之一。

负责：

- 输入（`Input`）；
- 创建 UI；
- 摄影机控制；
- 切换输入模式（UI / 游戏）。

示例：

**在菜单中**
- `PC_Menu`
- 开启 `Show Mouse Cursor`
- `Set Input Mode UI Only`

**在游戏中**
- `PC_Gameplay`
- `Game Only` 或 `Game and UI`

---

### 游戏状态类

`GameState` **同时存在于服务器和客户端上**。

用途：

- 计时器；
- 当前比赛阶段；
- 游戏的全局状态。

例如：

- `Server_GameState`

即使在单人模式下，也建议将数据保存在 `GameState` 中而非 `GameMode`。

---

### 玩家状态类

`PlayerState` 为每名玩家单独存在。

包含信息：

- 分数；
- 名称；
- 团队；
- 特权；
- 统计数据。

用途：

- 多人游戏 - 强制要求；
- 单人游戏 - 推荐使用。

---

### 观察者类

当玩家：死亡、观察或没有激活的 `Pawn` 时使用的 `Pawn`。

默认 `SpectatorPawn` 是推荐选择。

---

## 高级（GameMode）

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced.png"/>
</div>

### 全局服务器默认 GameMode

仅用于**专用服务器（dedicated server）**。

如果指定：

- 服务器将始终使用此 `GameMode`；
- 与地图无关。

通常为：

- `None` - 为标准选项；
- 在服务器打包中应用。

---

### 游戏模式地图前缀

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>

通过地图前缀自动分配 `GameMode`。

示例：

- `MP_` → `GM_Multiplayer`
- `SP_` → `GM_Singleplayer`
- `MENU_` → `GM_Menu`

#### 实践应用

- 可在同一构建中，自动适配不同模式。

在中型和大型项目中非常实用。

### 在 DefaultEngine.ini 中的配置

```ini
[/Script/EngineSettings.GameMapsSettings]
+GameModeMapPrefixes=(Prefix="MENU_",GameMode="/Game/GameModes/GM_Menu.GM_Menu_C")
+GameModeMapPrefixes=(Prefix="SP_",GameMode="/Game/GameModes/GM_Single.GM_Single_C")
+GameModeMapPrefixes=(Prefix="MP_",GameMode="/Game/GameModes/GM_Multiplayer.GM_Multiplayer_C")
+GameModeMapPrefixes=(Prefix="COOP_",GameMode="/Game/GameModes/GM_Coop.GM_Coop_C")
```

---

### Game Mode 类别别名配置

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Aliases.png"/>
</div>

此功能允许为 `GameMode` 使用便捷的简短别名，特别是在地图相同但游戏规则不同的情况下。

---

### 实践中的应用

#### 通过控制台或命令行使用

```ini
open Lvl_Arena?game=DM
```

Unreal Engine 会在 `Game Mode Class Aliases` 中查找 `DM`，并用 `GM_Deathmatch` 替换默认 `GameMode`。

#### 通过服务器启动

```ini
UEGameServer.exe Lvl_Map?game=TDM?listen
```
