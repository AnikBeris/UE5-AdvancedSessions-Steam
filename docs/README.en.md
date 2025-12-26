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
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=Stars&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
Useful information for project development on Unreal Engine 5 using the AdvancedSessions-Steam plugin
</h1>

<h2 align="center">
> 💡 The material is targeted at prepared users.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Disclaimer ⚠️
</h2>

<p align="center">
  The author is not responsible for any possible consequences of using this project.<br>
  Use it at your own risk.
</p>

<details align="center"> 
    <summary>⚠️Full Text⚠️</summary>
    
Use the materials of this repository at your own risk.

1. By using the materials of this repository, you automatically agree to the associated license terms.

2. The author provides no warranties, explicit or implied, regarding the accuracy, completeness, or suitability of these materials for any particular purposes. 
   
3. The author is not liable for any damages, including but not limited to direct, indirect, incidental, consequential, or special damages arising from the use or inability to use the materials from this repository or the accompanying documentation, even if you were previously informed of the possibility of such damages.

4. By using these materials, you acknowledge and assume all risks associated with their application. Furthermore, you agree that the author cannot be held responsible for any issues or consequences resulting from their use.

</details> 

---

<h3 align="center"> 
💖 Support the project 
</h3>

<p align="center"> 
If this project has been useful to you, consider giving it a star.:star2: 
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
Donations are warmly welcomed, no matter how small, and thank you so much. 😌 
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
  <sub> Thank you for your attention to the project and for your support 💙 </sub>
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



## 📊 Installed Plugins

<details> 
    <summary>⚙️ Expand Description</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Plugin Deactivation

<details> 
    <summary>⚙️ Expand Description</summary>

- **SteamSockets:** The SteamSockets plugin driver is required for Steam to work, but within the framework of the Advanced Sessions Plugin, it needs to be disabled.

</details> 



## 📊 Functions || Features

<details> 
    <summary>⚙️ Expand Description</summary>



</details>


# Project - Maps & Modes

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Section Purpose

The **Project - Maps & Modes** section defines key entry points for the game flow and project architecture. It configures:

---

- which `GameMode` is used by default;
- which maps are loaded when the editor, game, and server start;
- what base classes are applied (`Pawn`, `Controller`, `HUD` etc.);
- how to automatically switch `GameMode` depending on the map or its prefix.

Essentially, this is the **entry point into the game flow architecture**.

---

# Default Modes

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Default GameMode.png"/>
</div>


## Default GameMode

**Default GameMode** is the `GameMode` that will be used:

- if the map does not override `GameMode`;
- if the `GameMode` is not specified via URL parameters;
- if prefixes or aliases do not apply.


#### Typical Usage

- `GM_Menu` - main menu
- `GM_Gameplay` - main game
- `GM_Lobby` - multiplayer lobby

#### Important

- `GameMode` exists **only on the server** (or in single-player as server-authority).
- Clients receive data via the `GameState`.

---

## Selected GameMode

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

This block sets a set of classes for the selected `GameMode` (in this case `GM_Menu`).

---

### Default Pawn Class

Specifies which `Pawn` will be automatically spawned for the player.

Examples:

- `Pawn` - a placeholder for the menu
- `Character` - if a full-fledged character is needed
- `SpectatorPawn` - if the player should not control a body

For menus:

- a blank `Pawn` or minimal logic without control is often used.

---

### HUD Class

The `HUD` class (deprecated but still supported).

Used when:

- UI is drawn through `DrawHUD`;
- old HUD logic is applied.

Modern practice:

- the `HUD` is empty;
- UI is created via **UMG** in `PlayerController`.

Using `HUD_Menu` for menus is acceptable.

---

### Player Controller Class

One of the key architecture classes.

Responsible for:

- input (`Input`);
- creating UI;
- camera control;
- switching input modes (UI / Game).

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

`GameState` exists **on the server and clients**.

Used for:

- timers;
- current match phase;
- global game state.

Example:

- `Server_GameState`

Even in single-player, it is recommended to store data in `GameState` rather than in `GameMode`.

---

### Player State Class

`PlayerState` exists for each player.

Stores:

- scores;
- name;
- team;
- perks;
- stats.

Usage:

- required in multiplayer;
- recommended in single-player.

---

### Spectator Class

`Pawn` used:

- on death;
- when observing;
- when no active `Pawn` is present.

By default, `SpectatorPawn` is a correct choice.

---

## Advanced (GameMode)

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced.png"/>
</div>

### Global Default Server Game Mode

Used **only for the dedicated server**.

If specified:

- the server will always use this `GameMode`;
- regardless of the map.

Usually:

- `None` - the standard option;
- applied in server builds.

---

### Game Mode Map Prefixes

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>

Allows automatic assignment of `GameMode` based on the map prefix.

Example:

- `MP_` -> `GM_Multiplayer`
- `SP_` -> `GM_Singleplayer`
- `MENU_` -> `GM_Menu`

#### Practical Use

- one build;
- different modes without manual map setup.

Extremely useful in mid-sized and large projects.

### Setup in DefaultEngine.ini

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
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Aliases.png"/>
</div>

Enables using short aliases for `GameMode` when the maps stay the same but the game rules differ.

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

Lobby and service modes:

- `"MENU"`  -> `GM_Menu`
- `"LOBBY"` -> `GM_Lobby`
- `"ENTRY"` -> `GM_Entry`

Single-player mode:

- `"SP"`       -> `GM_Singleplayer`
- `"STORY"`    -> `GM_Story`
- `"CAMPAIGN"` -> `GM_Campaign`


### Setup in DefaultEngine.ini

```ini
[/Script/EngineSettings.GameMapsSettings]
+GameModeClassAliases=(ShortName="DM",GameMode="/Game/GameModes/GM_Deathmatch.GM_Deathmatch_C")
+GameModeClassAliases=(ShortName="TDM",GameMode="/Game/GameModes/GM_TeamDeathmatch.GM_TeamDeathmatch_C")
+GameModeClassAliases=(ShortName="COOP",GameMode="/Game/GameModes/GM_Coop.GM_Coop_C")
+GameModeClassAliases=(ShortName="MENU",GameMode="/Game/GameModes/GM_Menu.GM_Menu_C")
```


## Practical Application
### Via Console or Command Line

```ini
open Lvl_Arena?game=DM
```

Unreal Engine looks for `DM` in `Game Mode Class Aliases`, ignores the assigned `Default GameMode`, and replaces it with `GM_Deathmatch`,


### Via Server Startup

```ini
UEGameServer.exe Lvl_Map?game=TDM?listen
```

### Very convenient for:

- dedicated servers,
- CI/CD,
- automated tests.

---

### When aliases are NOT needed

Aliases are not mandatory if you use:

- `Map Override` in World Settings,
- `Game Mode Map Prefixes`,
- strictly fixed `Default GameMode`.

> In small single-player projects, aliases are often not used at all.


### Recommended scheme for a real project

Use all three mechanisms as intended:
|Mechanism|For what purpose|
|:---------:|:---------|
| Default GameMode | Safe fallback |
| Map Override | Explicit map behavior |
| Prefixes | Mass maps |
| Aliases | CLI, server, automation |

---






## Default Maps

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/Default Maps.png"/>
</div>

### Editor Startup Map

The map that:

- loads automatically when the editor starts.

Recommendation:

- a lightweight map;
- not the main game scene;
- often a test or menu.

---

### Editor Template Map Overrides

Rarely used.

Purpose:

- override built-in template maps;
- relevant for custom templates.

Not used in most projects.

---

### Game Default Map

The map that:

- loads at game launch;
- used in packaged builds.

Usually:

- the main menu;
- or the starting level.

---

## Advanced (Maps)

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/Default Maps - Advanced.png"/>
</div>

### Local Map Options

Allows default URL parameters to be specified.

Example:

```ini
?listen?game=GM_Gameplay
```

Used for:

- testing;
- local servers;
- automatic startup parameters.

---

### Transition Map

A map that:

- temporarily loads during level changes (Seamless Travel).

Used in multiplayer to:

- avoid freezes;
- provide a smooth transition between levels.

Usually not required in single-player.

---

### Server Default Map

The map that:

- loads when the dedicated server starts up.

Usually:

- `Entry`;
- or `Lvl_Lobby`.

Important:

- does not affect the client;
- only applies to server builds.

---

### Setup in DefaultEngine.ini

```ini
[/Script/EngineSettings.GameMapsSettings]
GameDefaultMap=/Game/Maps/MENU_Main
EditorStartupMap=/Game/Maps/Test_Map
GlobalDefaultGameMode=/Game/GameModes/GM_Menu.GM_Menu_C

```
## Practical Recommendations for the Current Structure

Typical configuration schema:

- **Editor Startup Map** -> `TestMap`
- **Game Default Map**   -> `Lvl_Menu`
- **Default GameMode**   -> `GM_Menu`
- **Menu Map Override**  -> `GM_Menu`
- **Gameplay Maps**      -> `GM_Gameplay` (via Override or Prefix)

This scheme ensures clear separation of menu, gameplay, and server logic, as well as simplifying project scalability.





* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 


<h2 align="center">
  <a href="#-table-of-contents">⬆️ Back to Top</a> 
</h2>

# Create Session 

<h1 align="center"> 
Create Session with Predefined Settings
</h1>

<details> 
    <summary> ⚙️ Expand Description </summary>

```
ServerName
```

```
ServerMap
```

```
GameMode
```

<div align="center">
  <img style="width: 50%; height: auto;" alt="CreateSession" src=".Tutorial\Article_2\CreateSession.png"/>
</div>

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

# Find Session

<h1 align="center"> 
Find Session with Predefined Settings
</h1>

<details> 
    <summary> ⚙️ Expand Description </summary>

```
ServerName
```

```
ServerMap
```

```
GameMode
```

<div align="center">
  <img style="width: 50%; height: auto;" alt="FindSession" src=".Tutorial\Article_2\FindSession.png"/>
</div>

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

# PlayerName PlayerNickname

<h1 align="center"> 
PlayerName | PlayerNickname
</h1>

<details> 
    <summary> ⚙️ Expand Description </summary>

```sh
HOSTING MATCH
```

```sh
CLIENT
```

```sh
SOLO PLAY
```

<div align="center">
  <img style="width: 50%; height: auto;" alt="PlayerName PlayerNickname" src=".Tutorial\Article_2\PlayerNamePlayerNickname.png"/>
</div>

</details>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

# Checks

<h1 align="center"> 
Is Server -> Is Standalone -> Set Text
</h1>

<details> 
    <summary> ⚙️ Expand Description </summary>

```sh
HOSTING MATCH
```

```sh
CLIENT
```

```sh
SOLO PLAY
```

<div align="center">
  <img style="width: 50%; height: auto;" alt="IsServer-IsStandalone-SetText" src=".Tutorial\Article_3\IsServer-IsStandalone-SetText.png"/>
</div>

</details>


<h1 align="center"> 
Has Online Subsystem - Which Subsystem is Active
</h1>

<details> 
    <summary> ⚙️ Expand Description </summary>

```sh
Steam
```

```sh
EOS
```

```sh
NULL
```

<div align="center">
  <img style="width: 50%; height: auto;" alt="HasOnlineSubsystem" src=".Tutorial\Article_3\HasOnlineSubsystem.png"/>
</div>

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 











<h1 align="center"> 📜 License </h1>
<p align="center">
  <strong> This project is distributed under </strong> 
  <a href="/LICENSE">Apache License</a> 
</p>

---

<h2 align="center"> 
Documentation - Please Review It 
</h2>

<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Spanish</a> |
  <a href="/docs/README.zh.md">Chinese</a> |
  <strong><-------</strong>
</p>


<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Spanish</a> |
  <a href="/docs/README.zh.md">Chinese</a> |
  <strong><-------</strong>
</p>
