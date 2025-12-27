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
Useful Information about Developing a Project on Unreal Engine 5 using the AdvancedSessions-Steam Plugin
</h1>

<h2 align="center">
> 💡 The material is intended for advanced users.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Disclaimer ⚠️
</h2>

<p align="center">
  The author shall not be held responsible for any consequences arising from the use of this project.<br>
  Use at your own risk.
</p>

<details align="center"> 
    <summary>⚠️Full text⚠️</summary>
    
Use the materials of this repository at your own risk.

1. By using the materials of this repository, you automatically agree to the terms of the license agreement associated with it.

2. The author makes no warranties, express or implied, regarding the accuracy, completeness, or suitability of these materials for any specific purpose. 
   
3. The author shall not be held responsible for any damages, including but not limited to direct, indirect, incidental, consequential, or special damages arising from the use or inability to use the materials from this repository or accompanying documentation, even if informed in advance about the possibility of such damages.

4. By using the materials of this repository, you acknowledge and accept all risks associated with its application. Moreover, you agree that the author cannot be held responsible for any issues or consequences arising from its use.

</details> 

---

<h3 align="center"> 
💖 Support the Project 
</h3>

<p align="center"> 
If you found this project useful, consider giving it a star.:star2: 
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
Donations are warmly appreciated, no matter how small. Thank you kindly. 😌 
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



## 📚 Table of Contents

- [Introduction](#-introduction)




## 🔗 Useful Links

  

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-table-of-contents"> ⬆️ Back to Top </a> 
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

- **SteamSockets:** SteamSockets plugin driver is required for Steam to work but must be disabled for Advanced Sessions Plugin.

</details> 



## 📊 Features || Highlights

<details> 
    <summary>⚙️ Expand Description</summary>



</details>


<h2 align="center">
  <a href="#-table-of-contents">⬆️ Back to Top</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Section Purpose

The **Project - Maps & Modes** section defines key entry points into the game flow and project architecture. It configures:

---

- which `GameMode` is used by default;
- which maps are loaded when starting the editor, game, and server;
- which base classes are applied (`Pawn`, `Controller`, `HUD`, etc.);
- how to automatically substitute `GameMode` depending on a map or its prefix.

Essentially, this is the **entry point into the game's architecture**.

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-table-of-contents">⬆️ Back to Top</a> 
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

- if the level does not override the `GameMode`;
- if the `GameMode` is not specified via URL parameters;
- if prefixes or aliases do not apply.

#### Typical Usage

- `GM_Menu` - main menu
- `GM_Gameplay` - core gameplay
- `GM_Lobby` - multiplayer lobby

#### Important

- `GameMode` exists **only on the server** (or in singleplayer as server-authority).
- Clients receive data via `GameState`.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-table-of-contents">⬆️ Back to Top</a> 
</h2>

###### # Selected GameMode

<h1 align="center"> 
Selected GameMode
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

**Selected GameMode** - This block determines the class set for the selected `GameMode` (in this case, `GM_Menu`).

<details> 
    <summary> ⚙️ Expand Description </summary>
---

### Default Pawn Class

Specifies which `Pawn` will be automatically spawned for the player.

Examples:

- `Pawn` - basic for menus
- `Character` - for full-fledged player characters
- `SpectatorPawn` - for observer roles

For menus:

- often a simple `Pawn` or minimal logic without control.

---

### HUD Class

`HUD` class (deprecated but still supported).

Used if:

- UI is drawn via `DrawHUD`;
- older HUD logic is applied.

Modern practice:

- Empty `HUD`;
- UI is created through **UMG** in `PlayerController`.

Using `HUD_Menu` for menus is acceptable.

---

### Player Controller Class

One of the key architecture classes.

Responsible for:

- input handling;
- creating UI;
- camera control;
- switching input modes (UI / Game).

Examples:

**For menu**
- `PC_Menu`
- `Show Mouse Cursor` enabled
- `Set Input Mode UI Only`

**For gameplay**
- `PC_Gameplay`
- `Game Only` or `Game and UI`

---

### Game State Class

`GameState` exists **on the server and clients**.

Used for:

- timers;
- match phases;
- global game state.

Example:

- `Server_GameState`

Even in singleplayer, it's recommended to store data in `GameState` rather than `GameMode`.

---

### Player State Class

`PlayerState` exists for each player.

Stores:

- score;
- name;
- team;
- perks;
- stats.

Usage:

- mandatory for multiplayer;
- recommended for singleplayer.

---

### Spectator Class

`Pawn` used:

- after death;
- for observation;
- if no active `Pawn` is present.

Default `SpectatorPawn` is a valid choice.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-table-of-contents">⬆️ Back to Top</a> 
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

### Global Default Server Game Mode

- Used **only for dedicated server**.

If set:

- the server will always use this `GameMode`;
- regardless of the map.

Usually:

- `None` - the standard option;
- applied in server builds.

---

### Game Mode Map Prefixes

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Prefixes" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-PrefixesLevel" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>


Allows automatic `GameMode` assignment based on map prefix.

Example:

- `MP_` -> `GM_Multiplayer`
- `SP_` -> `GM_Singleplayer`
- `MENU_` -> `GM_Menu`

#### Practical Application

- single build for multiple modes;
- no manual map configurations needed.

Highly useful in medium and large projects.

### Configuration in DefaultEngine.ini

```ini
[/Script/EngineSettings.GameMapsSettings]
+GameModeMapPrefixes=(Prefix="MENU_",GameMode="/Game/GameModes/GM_Menu.GM_Menu_C")
+GameModeMapPrefixes=(Prefix="SP_",GameMode="/Game/GameModes/GM_Single.GM_Single_C")
+GameModeMapPrefixes=(Prefix="MP_",GameMode="/Game/GameModes/GM_Multiplayer.GM_Multiplayer_C")
+GameModeMapPrefixes=(Prefix="COOP_",GameMode="/Game/GameModes/GM_Coop.GM_Coop_C")

```

---

### Game Mode Class Aliases

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Aliases" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Aliases.png"/>
</div>

Allows short aliases for `GameMode`. When maps are the same but game rules vary.

Classic PvP example:

- `"DM"`   -> `GM_Deathmatch`
- `"TDM"`  -> `GM_TeamDeathmatch`
- `"CTF"`  -> `GM_CaptureTheFlag`
- `"FFA"`  -> `GM_FreeForAll`
- `"KOTH"` -> `GM_KingOfTheHill`
- `"SD"`   -> `GM_SearchAndDestroy`

Classic PvE example:

- `"COOP"`  -> `GM_Coop`
- `"PVE"`   -> `GM_PvE`
- `"SURV"`  -> `GM_Survival`
- `"HORDE"` -> `GM_Horde`
- `"WAVES"` -> `GM_Waves`




