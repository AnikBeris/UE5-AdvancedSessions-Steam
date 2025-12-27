<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Russian</a> |
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
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=Stars&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
Useful Information on Developing a Project in Unreal Engine 5 Using the AdvancedSessions-Steam Plugin
</h1>

<h2 align="center">
> 💡 This material is intended for advanced users.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Disclaimer ⚠️
</h2>

<p align="center">
  The author is not responsible for any possible consequences resulting from the use of this project.<br>
  Use at your own risk.
</p>

<details align="center"> 
    <summary>⚠️full text⚠️</summary>
    
Use the materials of this repository at your own risk.

1. By using the materials of this repository, you automatically agree to the terms of the licensing agreement associated with it.

2. The author does not provide any guarantees, explicit or implied, regarding the accuracy, completeness, or suitability of these materials for any particular purpose. 
   
3. The author is not responsible for any damage, including but not limited to direct, indirect, incidental, consequential, or special damage arising from the use or inability to use the materials from this repository or its accompanying documentation, even if prior notification of such possible damage was given.

4. By using the materials of this repository, you acknowledge and assume all risks associated with its application. Furthermore, you agree that the author cannot be held responsible for any problems or consequences resulting from its use.

</details> 

---

<h3 align="center"> 
💖 Support the Project 
</h3>

<p align="center"> 
If this project has been useful to you, you can rate it by giving it a star.:star2: 
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
Donations are warmly welcomed, no matter how small, and thank you very much. 😌 
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
  <sub> Thank you for your attention to the project and support 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



## 📚 Contents

- [Introduction](#-introduction)




## 🔗 Useful Links

  

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contents"> ⬆️ Back to Top </a> 
</h2>

<h1 align="center"> 
Technical Requirements
</h1>



## 📊 Installed Plugin

<details> 
    <summary>⚙️ Expand Description</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Disabling Plugins

<details> 
    <summary>⚙️ Expand Description</summary>

- **SteamSockets:** The SteamSockets driver plugin is necessary for Steam functionality, but within the context of Advanced Sessions Plugin, it needs to be disabled.

</details> 



## 📊 Features || Functions

<details> 
    <summary>⚙️ Expand Description</summary>



</details>


<h2 align="center">
  <a href="#-contents">⬆️ Back to Top</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Section Purpose

The **Project - Maps & Modes** section defines key entry points into the game flow and project architecture. It configures the following:

---

- which `GameMode` is used by default;
- which maps load at the start of the editor, game, and server;
- which base classes are applied (`Pawn`, `Controller`, `HUD`, etc.);
- how to automatically switch `GameMode` depending on the map or its prefix.

Essentially, this is the **entry point into the game flow architecture**.

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contents">⬆️ Back to Top</a> 
</h2>

###### # Default Modes

<h1 align="center"> 
Default Modes
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Default GameMode.png"/>
</div>

## Default GameMode

<details>
    <summary> ⚙️ Expand Description </summary>

**Default GameMode** is the `GameMode` that will be used:

- if the map does not override `GameMode`;
- if `GameMode` is not specified via URL parameters;
- if prefixes or aliases do not trigger.

#### Typical Use

- `GM_Menu` - main menu
- `GM_Gameplay` - main game
- `GM_Lobby` - multiplayer lobby

#### Important

- `GameMode` exists **only on the server** (or in singleplayer, as server-authority).
- Clients receive data via `GameState`.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contents">⬆️ Back to Top</a> 
</h2>

###### # Selected GameMode

<h1 align="center"> 
Selected GameMode
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

**Selected GameMode** - This block defines a set of classes for the selected `GameMode` (in this case, `GM_Menu`).

<details> 
    <summary> ⚙️ Expand Description </summary>
---

### Default Pawn Class

Determines which `Pawn` will be automatically spawned for the player.

Examples:

- `Pawn` - placeholder for menu
- `Character` - if a full-fledged character is required
- `SpectatorPawn` - if the player should not control a body

For menus:

- often an empty `Pawn` or minimal logic without control is used.

---

### HUD Class

`HUD` class (deprecated, but still supported).

Used when:

- UI is drawn through `DrawHUD`;
- older HUD logic is applied.

Modern practice:

- `HUD` is empty;
- UI is created using **UMG** in `PlayerController`.

For menus, using `HUD_Menu` is acceptable.

--- 

(...translation continues...)
