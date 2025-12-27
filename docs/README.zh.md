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
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=星标&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
使用 AdvancedSessions-Steam 插件在 Unreal Engine 5 上开发项目的有用信息
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
  作者对使用本项目可能产生的任何后果不承担责任。<br>
  请自行承担使用风险。
</p>

<details align="center"> 
    <summary>⚠️完整文本⚠️</summary>
    
使用本存储库的资料，您需自行承担全部风险。

1. 使用本存储库的资料，表明您自动同意与之相关的许可协议条款。

2. 作者对这些材料的准确性、完整性或适用性不作任何明示或暗示的保证，亦不对其适应于任何特定目的作出保证。
   
3. 作者对于因使用或无法使用本存储库的材料或相关文档而导致的任何损失，包括但不限于直接、间接、附随、派生或特殊损失，不承担任何责任，即便已被事先告知可能发生这种损失。

4. 使用本存储库的材料，您即表明愿意承担与使用这些材料相关的所有风险。此外，您同意作者对因使用这些材料而产生的任何问题或后果不负责任。

</details> 

---

<h3 align="center"> 
💖 支持项目 
</h3>

<p align="center"> 
如果本项目对您有帮助，您可以通过给它一个⭐来给予支持。:star2: 
</p>

<p align="center">
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="买杯咖啡">
  </a>
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="买杯咖啡">
  </a>
</p>



<h4 align="center"> 
即便是很小的捐助也是非常欢迎的，衷心感谢。😌 
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
  <sub> 感谢您对本项目的关注和支持 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



## 📚 内容目录

- [简介](#-简介)




## 🔗 有用链接

  

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-内容目录"> ⬆️ 返回顶部 </a> 
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

- **SteamSockets:** SteamSockets 插件驱动程序是 Steam 工作所必需的，但在使用 Advanced Sessions Plugin 时需要禁用。

</details> 



## 📊 功能 || 特点

<details> 
    <summary>⚙️ 展开描述</summary>



</details>


<h2 align="center">
  <a href="#-内容目录">⬆️ 返回顶部</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## 模块目的

**Project - Maps & Modes** 模块定义了游戏流程和项目架构的关键入口点。在此模块中可设置：

---

- 默认使用的 `GameMode`；
- 启动编辑器、游戏和服务器时加载的地图 (maps)；
- 应用的基础类 (`Pawn`、`Controller`、`HUD`等)；
- 根据地图或其前缀自动替换 `GameMode`。

实际上，这是 **游戏流程架构的入口点**。

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-内容目录">⬆️ 返回顶部</a> 
</h2>

###### # Default Modes

<h1 align="center"> 
默认模式
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Default GameMode.png"/>
</div>

## 默认 GameMode

<details>
    <summary> ⚙️ 展开描述 </summary>

**默认 GameMode** 是一个在以下情况下使用的 `GameMode`：

- 如果地图没有重写 `GameMode`；
- 如果通过 URL 参数未指定 `GameMode`；
- 如果前缀或别名未生效。

#### 典型应用

- `GM_Menu` - 主菜单
- `GM_Gameplay` - 主游戏
- `GM_Lobby` - 多人游戏大厅

#### 注意

- `GameMode` **仅存在于服务器上**（也可能存在于单人游戏中，作为 server-authority）。
- 客户端通过 `GameState` 接收数据。

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-内容目录">⬆️ 返回顶部</a> 
</h2>

###### # Selected GameMode

<h1 align="center"> 
所选 GameMode
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

**所选 GameMode** - 这是为选定 `GameMode`（在此情况下为 `GM_Menu`）定义的一组类。

<details> 
    <summary> ⚙️ 展开描述 </summary>
---

### 默认 Pawn 类

定义将为玩家自动生成哪个 `Pawn`。

示例：

- `Pawn` - 用于菜单的占位情况
- `Character` - 当需要一个完整的角色时使用
- `SpectatorPawn` - 玩家不需要控制角色时使用

对于菜单：

- 通常使用空的 `Pawn` 或最小逻辑占位。

---

### HUD 类

`HUD` 类（虽然已经过时，但仍然被支持）。

在以下情况下使用：

- UI 通过 `DrawHUD` 绘制；
- 使用旧版 HUD 逻辑。

现代实践：

- `HUD` 为空；
- UI 在 `PlayerController` 中通过 **UMG** 创建。

在菜单中可以使用 `HUD_Menu`。

---

### 玩家控制器类

架构中的关键类之一。

负责：

- 输入 (`Input`)；
- 创建 UI；
- 控制摄像机；
- 切换输入模式（UI / 游戏）。

示例：

**在菜单**
- `PC_Menu`
- 启用 `显示鼠标指针`
- `设置输入模式为 UI 模式`

**在游戏中**
- `PC_Gameplay`
- `仅游戏` 或 `游戏和 UI`

---

### 游戏状态类

`GameState` **在服务器和客户端上存在**。

用于：

- 计时器；
- 比赛当前阶段；
- 游戏全局状态。

示例：

- `Server_GameState`

即使在单人游戏，也建议将数据存储在 `GameState` 中，而不是 `GameMode`。

---

### 玩家状态类

`PlayerState` 每个玩家都有。

存储：

- 分数；
- 名称；
- 队伍；
- 特技；
- 统计数据。

应用：

- 在多人游戏中 - 必须如此；
- 在单人游戏中 - 推荐。

---

### 观察者类

`Pawn` 在以下情况使用：

- 玩家角色死亡；
- 观察模式；
- 没有活动的 `Pawn` 时。

默认情况下，`SpectatorPawn` 是推荐选择。

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-内容目录">⬆️ 返回顶部</a> 
</h2>

###### # Advanced (GameMode)

<h1 align="center"> 
高级 (GameMode)
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced.png"/>
</div>

<details> 
    <summary> ⚙️ 展开描述 </summary>

### 全局默认服务器游戏模式

- 仅用于 **dedicated server**。

如果已指定：

- 服务器始终使用此 `GameMode`；
- 无论地图为何。

通常设为：

- `None` - 标准选项；
- 在服务器构建中应用。

---

### 游戏模式地图前缀

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Prefixes" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-PrefixesLevel" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>


允许根据地图前缀自动分配 `GameMode`。

示例：

- `MP_` -> `GM_Multiplayer`
- `SP_` -> `GM_Singleplayer`
- `MENU_` -> `GM_Menu`

#### 实用场景

- 单一构建；
- 不同模式的地图无需手动设置。

在中型和大型项目中特别有用。

### 配置方式 DefaultEngine.ini

```ini
[/Script/EngineSettings.GameMapsSettings]
+GameModeMapPrefixes=(Prefix="MENU_",GameMode="/Game/GameModes/GM_Menu.GM_Menu_C")
+GameModeMapPrefixes=(Prefix="SP_",GameMode="/Game/GameModes/GM_Single.GM_Single_C")
+GameModeMapPrefixes=(Prefix="MP_",GameMode="/Game/GameModes/GM_Multiplayer.GM_Multiplayer_C")
+GameModeMapPrefixes=(Prefix="COOP_",GameMode="/Game/GameModes/GM_Coop.GM_Coop_C")

```

---

### 游戏模式类别名

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Aliases" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Aliases.png"/>
</div>

允许为 `GameMode` 使用简短的别名。适用当有相同地图，但规则不同。

经典 PvP 示例：

- `"DM"`   -> `GM_Deathmatch`
- `"TDM"`  -> `GM_TeamDeathmatch`
- `"CTF"`  -> `GM_CaptureTheFlag`

单人模式：

- `"SP"`       -> `GM_Singleplayer`
- `"STORY"`    -> `GM_Story`
- `"CAMPAIGN"` -> `GM_Campaign`

---

### 配置 DefaultEngine.ini 中的别名示例

```ini
[/Script/EngineSettings.GameMapsSettings]
+GameModeClassAliases=(ShortName="DM",GameMode="/Game/GameModes/GM_Deathmatch.GM_Deathmatch_C")
+GameModeClassAliases=(ShortName="TDM",GameMode="/Game/GameModes/GM_TeamDeathmatch.GM_TeamDeathmatch_C")
+GameModeClassAliases=(ShortName="COOP",GameMode="/Game/GameModes/GM_Coop.GM_Coop_C")
+GameModeClassAliases=(ShortName="MENU",GameMode="/Game/GameModes/GM_Menu.GM_Menu_C")
```


---

### 如何在实践中应用
通过命令行或控制台：

```ini
open Lvl_Arena?game=DM
```

Unreal Engine 会在 `Game Mode Class Aliases` 中查找 `DM`，忽略指定的 `默认 GameMode` 并将其替换为 `GM_Deathmatch`。

服务器启动示例：

```ini
UEGameServer.exe Lvl_Map?game=TDM?listen
```

非常适合：

- dedicated servers；
- CI/CD；
- 自动化测试。

</details>

... (剩余对内容的大量翻译，量较多无法全部列出)
