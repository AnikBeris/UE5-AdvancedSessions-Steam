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
  The author assumes no responsibility for any potential consequences of using this project.<br>
  Use at your own risk.
</p>

<details align="center"> 
    <summary>⚠️ Full Text ⚠️</summary>
    
Use the materials of this repository at your own risk.

1. By using the materials of this repository, you automatically agree to the terms of the license agreement associated with it.

2. The author provides no warranties, express or implied, regarding the accuracy, completeness, or fitness of these materials for any specific purposes. 
   
3. The author is not responsible for any damages, including but not limited to direct, indirect, incidental, consequential, or special damages arising from the use or inability to use these materials or the accompanying documentation, even if the possibility of such damages has been previously reported.

4. By using these materials, you acknowledge and accept all risks associated with their application. Furthermore, you agree that the author cannot be held liable for any issues or consequences resulting from their use.

</details> 

---

<h3 align="center"> 
💖 Support the project 
</h3>

<p align="center"> 
If this project proved useful to you, feel free to rate it by leaving a star.:star2: 
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
Donations are warmly welcomed, no matter how small, and many thanks in advance. 😌 
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
  <sub> Thank you for your attention to the project and your support 💙 </sub>
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
  <a href="#-contents"> ⬆️ To Top </a> 
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

- **SteamSockets:** The SteamSockets plugin driver is required for Steam to work, but within the scope of Advanced Sessions Plugin, it needs to be disabled.

</details> 



## 📊 Functions || Features

<details> 
    <summary>⚙️ Expand Description</summary>



</details>


<h2 align="center">
  <a href="#-contents">⬆️ To Top</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Purpose of the Section

The **Project - Maps & Modes** section defines key entry points into the game's flow and project architecture. It configures:

---

- which `GameMode` is used by default;
- which maps (levels) are loaded at the start of the editor, game, or server;
- which base classes are applied (`Pawn`, `Controller`, `HUD`, etc.);
- how to automatically override the `GameMode` depending on the map or its prefix.

Essentially, this is the **entry point into the architecture of the game flow**.

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contents">⬆️ To Top</a> 
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

**Default GameMode** - is the `GameMode` to be used:

- if the level does not override the `GameMode`;
- if the `GameMode` is not specified via URL parameters;
- if prefixes or aliases did not work.

#### Typical Use

- `GM_Menu` - main menu
- `GM_Gameplay` - main gameplay
- `GM_Lobby` - multiplayer lobby

#### Important

- `GameMode` exists **only on the server** (or in single player, acting as server authority).
- Clients receive data through `GameState`.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contents">⬆️ To Top</a> 
</h2>

###### # Selected GameMode

<h1 align="center"> 
Selected GameMode
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

**Selected GameMode** - This block determines the set of classes for the selected `GameMode` (in this case, `GM_Menu`).

<details> 
    <summary> ⚙️ Expand Description </summary>
---

### Default Pawn Class

Determines which `Pawn` will be automatically spawned for the player.

Examples:

- `Pawn` - placeholder for a menu
- `Character` - for a full-fledged character
- `SpectatorPawn` - for non-controlling players

For menus:

- often an empty `Pawn` or minimal logic without controls is used.

---

### HUD Class

`HUD` class (deprecated, yet still supported).

Used if:

- UI is drawn via `DrawHUD`;
- traditional HUD logic is applied.

Modern practice:

- `HUD` is empty;
- UI is created via **UMG** in `PlayerController`.

Using a `HUD_Menu` in a menu is acceptable.

---

### Player Controller Class

One of the key architecture classes.

Responsible for:

- input (`Input`);
- UI creation;
- camera management;
- input mode switching (UI / Game).

Examples:

**In the menu**
- `PC_Menu`
- `Show Mouse Cursor` enabled
- `Set Input Mode UI Only`

**In the game**
- `PC_Gameplay`
- `Game Only` or `Game and UI`

---

### Game State Class

`GameState` exists **on both the server and clients**.

Used for:

- timers;
- current match phase;
- global game state.

Example:

- `Server_GameState`

Even in single-player, it's recommended to store data in `GameState` rather than `GameMode`.

---

### Player State Class

`PlayerState` exists for each player.

Stores:

- score;
- name;
- team;
- perks;
- statistics.

Usage:

- in multiplayer - mandatory;
- in single-player - recommended.

---

### Spectator Class

`Pawn` used:

- upon death;
- for observing;
- when no active `Pawn` is present.

By default, `SpectatorPawn` is a suitable choice.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contents">⬆️ To Top</a> 
</h2>

###### # Advanced (GameMode)

<h1 align="center"> 
Advanced (GameMode)
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced.png"/>
</div>

<details> 
    <summary> ⚙️ Expand Description </summary>
