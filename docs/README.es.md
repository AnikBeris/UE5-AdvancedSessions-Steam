<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chino</a> |
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
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=Estrellas&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
Información útil sobre el desarrollo de un proyecto en Unreal Engine 5 utilizando el plugin AdvancedSessions-Steam
</h1>

<h2 align="center">
> 💡 El material está orientado a usuarios preparados.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Descargo de responsabilidad ⚠️
</h2>

<p align="center">
  El autor no se hace responsable de las posibles consecuencias del uso de este proyecto.<br>
  Use bajo su propia responsabilidad.
</p>

<details align="center"> 
    <summary>⚠️texto completo⚠️</summary>
    
Use el material de este repositorio bajo su propio riesgo.

1. Al usar el material de este repositorio, usted acepta automáticamente los términos del acuerdo de licencia asociados con el mismo.

2. El autor no garantiza de ninguna manera, ya sea explícita o implícitamente, la exactitud, integridad o idoneidad de estos materiales para fines específicos.
   
3. El autor no se hace responsable de ninguna pérdida, incluidos, entre otros, daños directos, indirectos, incidentales, consecuenciales o especiales, que resulten del uso o la imposibilidad de usar los materiales de este repositorio o la documentación asociada con el mismo, incluso si se le había informado previamente de la posibilidad de dichos daños.

4. Al usar el material de este repositorio, usted reconoce y asume todos los riesgos asociados con su aplicación. Además, acepta que el autor no puede ser responsable de ningún problema o consecuencia resultante de su uso.

</details> 

---

<h3 align="center"> 
💖 Apoya el proyecto 
</h3>

<p align="center"> 
Si este proyecto te fue útil, puedes calificarlo con una estrella.:star2: 
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
Las donaciones son muy bien recibidas, no importa lo pequeñas que sean, y muchas gracias. 😌 
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
  <sub> Gracias por tu atención al proyecto y por el apoyo 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



## 📚 Contenido

- [Introducción](#-introducción)




## 🔗 Enlaces útiles

  

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contenido"> ⬆️ Arriba </a> 
</h2>

<h1 align="center"> 
Requisitos técnicos
</h1>



## 📊 Plugin instalado

<details> 
    <summary>⚙️ Desplegar descripción</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Desactivación de plugins

<details> 
    <summary>⚙️ Desplegar descripción</summary>

- **SteamSockets:** El controlador del plugin SteamSockets es necesario para que Steam funcione, pero dentro del marco de Advanced Sessions Plugin debe desactivarse.

</details> 



## 📊 Funciones || Características

<details> 
    <summary>⚙️ Desplegar descripción</summary>



</details>


<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Propósito de la sección

La sección **Project - Maps & Modes** define los puntos clave de entrada en el flujo de juego y la arquitectura del proyecto. En esta sección se configura:

---

- qué `GameMode` se usa por defecto;
- qué maps (mapas) se cargan al inicio del editor, juego y servidor;
- qué clases base se aplican (`Pawn`, `Controller`, `HUD`, etc.);
- cómo cambiar automáticamente el `GameMode` dependiendo del mapa o su prefijo.

De hecho, esta es la **puerta de entrada a la arquitectura del flujo del juego**.

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 




<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
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
    <summary align="center"> ⚙️ Desplegar descripción </summary>

**Default GameMode** - Es el `GameMode` que será usado:

- si el nivel no sobrescribe `GameMode`;
- si `GameMode` no ha sido indicado en los parámetros de URL;
- si no aplican ni prefijos ni alias.

#### Uso típico

- `GM_Menu` - menú principal.
- `GM_Gameplay` - el juego principal.
- `GM_Lobby` - el lobby multijugador.

#### Importante

- `GameMode` existe **solo en el servidor** (o en un solo jugador, como servidor autoritativo).
- Los clientes obtienen datos a través del `GameState`.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Selected GameMode

<h1 align="center"> 
Selected GameMode
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

**Selected GameMode** - Este bloque define el conjunto de clases para el `GameMode` seleccionado (en este caso, `GM_Menu`).

<details> 
    <summary  align="center"> ⚙️ Desplegar descripción </summary>
---

### Default Pawn Class

Determina qué `Pawn` será generado automáticamente para el jugador.

Ejemplos:

- `Pawn` - mínimo para el menú.
- `Character` - si se necesita un personaje completo.
- `SpectatorPawn` - si el jugador no debe manejar un cuerpo.

Para menús:

- se usa usualmente un `Pawn` vacío o lógica mínima sin control.

---

### HUD Class

Clase `HUD` (obsoleta, pero aún compatible).

Usado si:

- la IU se dibuja a través de `DrawHUD`;
- se aplica la antigua lógica de HUD.

Práctica contemporánea:

- `HUD` vacío;
- la interfaz de usuario se genera a través de **UMG** en `PlayerController`.

Para menús, el uso de `HUD_Menu` es aceptable.

---

### Player Controller Class

Una de las clases clave de la arquitectura.

Responsable de:

- Entrada (`Input`);
- Generación de la interfaz de usuario;
- Control de la cámara;
- Cambio de modos de entrada (UI / Game).

Ejemplos:

**En el menú**
- `PC_Menu`
- activado `Show Mouse Cursor`
- `Set Input Mode UI Only`

**En el juego**
- `PC_Gameplay`
- `Game Only` o `Game and UI`

---

### Game State Class

`GameState` existe **tanto en el servidor como en los clientes**.

Se utiliza para:

- temporizadores;
- fase actual de la partida;
- estado global del juego.

Ejemplo:

- `Server_GameState`

Incluso en un solo jugador, se recomienda almacenar datos en `GameState` en lugar de en `GameMode`.

---

### Player State Class

`PlayerState` existe para cada jugador.

Contiene:

- puntos;
- nombre;
- equipo;
- perks;
- estadísticas.

Aplicación:

- en modo multijugador - obligatorio;
- en modo de un solo jugador - recomendado.

---

### Spectator Class

`Pawn` que se usa:

- al morir;
- al observar;
- cuando no hay un `Pawn` activo.

Por defecto, `SpectatorPawn` es una elección adecuada.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Advanced (GameMode)

<h1 align="center"> 
Advanced (GameMode)
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced.png"/>
</div>

<details> 
    <summary  align="center"> ⚙️ Desplegar descripción </summary>

### Global Default Server Game Mode

- Solo se utiliza para **dedicated server**.

Si está configurado:

- el servidor siempre usará este `GameMode`;
- independientemente del mapa.

Usualmente:

- `None` - opción estándar;
- se aplica en compilaciones del servidor.

---

### Game Mode Map Prefixes

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Prefixes" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-PrefixesLevel" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>


Permite asignar automáticamente `GameMode` por prefijo de mapa.

Ejemplo:

- `MP_` -> `GM_Multiplayer`
- `SP_` -> `GM_Singleplayer`
- `MENU_` -> `GM_Menu`

#### Aplicación práctica

- una compilación;
- diferentes modos sin configuración manual de mapas.

Sumamente útil en proyectos medianos y grandes.

### Configuración en DefaultEngine.ini

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

Permite usar alias cortos para `GameMode`. Cuando los mapas son iguales, pero las reglas del juego son específicas.

Ejemplo clásico PvP:

- `"DM"`   -> `GM_Deathmatch`
- `"TDM"`  -> `GM_TeamDeathmatch`
- `"CTF"`  -> `GM_CaptureTheFlag`
- `"FFA"`  -> `GM_FreeForAll`
- `"KOTH"` -> `GM_KingOfTheHill`
- `"SD"`   -> `GM_SearchAndDestroy`

Ejemplo clásico PvE:

- `"COOP"`  -> `GM_Coop`
- `"PVE"`   -> `GM_PvE`
- `"SURV"`  -> `GM_Survival`
- `"HORDE"` -> `GM_Horde`
- `"WAVES"` -> `GM_Waves`

Lobbies y modos de servicio:

- `"MENU"`  -> `GM_Menu`
- `"LOBBY"` -> `GM_Lobby`
- `"ENTRY"` -> `GM_Entry`

Modo para un solo jugador:

- `"SP"`       -> `GM_Singleplayer`
- `"STORY"`    -> `GM_Story`
- `"CAMPAIGN"` -> `GM_Campaign`


### Configuración en DefaultEngine.ini

```ini
[/Script/EngineSettings.GameMapsSettings]
+GameModeClassAliases=(ShortName="DM",GameMode="/Game/GameModes/GM_Deathmatch.GM_Deathmatch_C")
+GameModeClassAliases=(ShortName="TDM",GameMode="/Game/GameModes/GM_TeamDeathmatch.GM_TeamDeathmatch_C")
+GameModeClassAliases=(ShortName="COOP",GameMode="/Game/GameModes/GM_Coop.GM_Coop_C")
+GameModeClassAliases=(ShortName="MENU",GameMode="/Game/GameModes/GM_Menu.GM_Menu_C")
```


## Aplicación práctica
### A través de consola o línea de comandos

```ini
open Lvl_Arena?game=DM
```

Unreal Engine busca `DM` en `Game Mode Class Aliases`, ignora el `Default GameMode` asignado y lo reemplaza por `GM_Deathmatch`,


### A través de Server Startup

```ini
UEGameServer.exe Lvl_Map?game=TDM?listen
```

### Muy útil para:

- servidores dedicados,
- CI/CD,
- pruebas automáticas.

---

### Cuando los alias NO son necesarios

Los alias no son obligatorios si utilizas:

- `Map Override` en World Settings,
- `Game Mode Map Prefixes`,
- `Default GameMode` estrictamente definido.

> En proyectos pequeños para un solo jugador, los alias a menudo no se utilizan.


### Esquema recomendado para un proyecto real

Utilizar los tres mecanismos, pero según su propósito:
|Mecanismo|Para qué|
|:---------:|:---------|
| Default GameMode | Fallback seguro |
| Map Override | Comportamiento específico del mapa |
| Prefixes | Mapas en masa |
| Aliases | CLI, servidor, automatización |

</details>

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 





<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Default Maps

<h1 align="center"> 
Default Maps
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="Default Maps" src="../media/Tutorial/Article_1/Default Maps.png"/>
</div>


<details> 
    <summary  align="center"> ⚙️ Desplegar descripción </summary>


### Editor Startup Map

Mapa que:

- Se abre automáticamente al iniciar el editor.

Recomendación:

- Un mapa ligero;
- No una escena principal del juego;
- A menudo se usa uno de prueba o el menú.

---

### Editor Template Map Overrides

Raramente utilizado.

Propósito:

- Sobrescribir las plantillas de mapas predeterminadas (template maps);
- Aplicable para plantillas personalizadas.

En la mayoría de los proyectos no se utiliza.

---

### Game Default Map

Mapa que:

- Se carga al iniciar el juego;
- Se usa en la build empaquetada.

Típicamente:

- el menú principal;
- o el nivel inicial.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 




<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Advanced (Maps)

<h1 align="center"> 
Advanced (Maps)
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="Default Maps - Advanced" src="../media/Tutorial/Article_1/Default Maps - Advanced.png"/>
</div>

<details> 
    <summary align="center"> ⚙️ Desplegar descripción </summary>

### Local Map Options

Permite introducir parámetros por defecto en la URL.

Ejemplo:

```ini
?listen?game=GM_Gameplay
```

Usado para:

- pruebas;
- servidores locales;
- parámetros de inicio automáticos.

---

### Transition Map

Mapa que:

- Se carga temporalmente al cambiar niveles (Seamless Travel).

Usado en multijugador:

- Para evitar pausas bruscas;
- Para transiciones suaves entre niveles.

En modo de un solo jugador, generalmente no se requiere.

---

### Server Default Map

Mapa que:

- se carga al iniciar el servidor dedicado.

Usualmente:

- `Entry`;
- o `Lvl_Lobby`.

Importante:

- No afecta al cliente;
- Solo aplicado en la compilación para servidor.

---

### Configuración en DefaultEngine.ini

```ini
[/Script/EngineSettings.GameMapsSettings]
GameDefaultMap=/Game/Maps/MENU_Main
EditorStartupMap=/Game/Maps/Test_Map
GlobalDefaultGameMode=/Game/GameModes/GM_Menu.GM_Menu_C

```
## Recomendación práctica para la estructura actual

Esquema típico de configuración:

- **Editor Startup Map** -> `TestMap`
- **Game Default Map**   -> `Lvl_Menu`
- **Default GameMode**   -> `GM_Menu`
- **Menu Map Override**  -> `GM_Menu`
- **Gameplay Maps**      -> `GM_Gameplay` (usando Override o Prefijo)

Este esquema asegura una separación clara entre el menú, el juego y la lógica del servidor, al mismo tiempo que simplifica la escalabilidad del proyecto.

</details> 




* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 


<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Create Session 

<h1 align="center"> 
Create Session con configuración previa
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="CreateSession" src="../media/Tutorial/Article_2/CreateSession.png"/>
</div>

<details> 
    <summary> ⚙️ Desplegar descripción </summary>

```
ServerName
```

```
ServerMap
```

```
GameMode
```

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

###### # Find Session

<h1 align="center"> 
Find Session con configuración previa
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="FindSession" src="../media/Tutorial/Article_2/FindSession.png"/>
</div>

<details> 
    <summary> ⚙️ Desplegar descripción </summary>

```
ServerName
```

```
ServerMap
```

```
GameMode
```

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

###### # PlayerName PlayerNickname

<h1 align="center"> 
PlayerName | PlayerNickname
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="PlayerNamePlayerNickname" src="../media/Tutorial/Article_2/PlayerNamePlayerNickname.png"/>
</div>

<details> 
    <summary> ⚙️ Desplegar descripción </summary>

```sh
HOSTING MATCH
```

```sh
CLIENT
```

```sh
SOLO PLAY
```

</details>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

###### # Verificaciones


###### # Is Server -> Is Standalone -> Set Text

<h1 align="center"> 
Is Server -> Is Standalone -> Set Text
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="IsServer-IsStandalone-SetText" src="../media/Tutorial/Article_2/IsServer-IsStandalone-SetText.png"/>
</div>

<details> 
    <summary> ⚙️ Desplegar descripción </summary>

```sh
HOSTING MATCH
```

```sh
CLIENT
```

```sh
SOLO PLAY
```

</details>

---

###### # Has Online Subsystem

<h1 align="center"> 
Has Online Subsystem, qué subsistema está activo
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="HasOnlineSubsystem" src="../media/Tutorial/Article_2/HasOnlineSubsystem.png"/>
</div>

<details> 
    <summary> ⚙️ Desplegar descripción </summary>

```sh
Steam
```

```sh
EOS
```

```sh
NULL
```

</details> 




* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 











<h1 align="center"> 📜 Licencia </h1>
<p align="center">
  <strong> Este proyecto se distribuye bajo la </strong> 
  <a href="/LICENSE">Apache License</a> 
</p>

---

<h2 align="center"> 
Documentación, revísala 
</h2>

<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chino</a> |
  <strong><-------</strong>
</p>


<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chino</a> |
  <strong><-------</strong>
</p>
