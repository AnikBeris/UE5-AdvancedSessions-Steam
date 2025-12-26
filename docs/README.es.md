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
    <img alt="Logotipo del proyecto" src="../media/logo-light.png" width="512" height="auto">
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
Información útil sobre el desarrollo de proyectos en Unreal Engine 5 utilizando el plugin AdvancedSessions-Steam
</h1>

<h2 align="center">
> 💡 Este material está orientado a usuarios con experiencia.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Exención de Responsabilidad ⚠️
</h2>

<p align="center">
  El autor no se responsabiliza de las posibles consecuencias derivadas del uso de este proyecto.<br>
  Úselo bajo su propio riesgo.
</p>

<details align="center"> 
    <summary>⚠️ Texto completo ⚠️</summary>
    
Utilice los materiales de este repositorio bajo su propio riesgo.

1. Al usar los materiales de este repositorio, usted acepta automáticamente las condiciones del acuerdo de licencia correspondiente.

2. El autor no garantiza explícita ni implícitamente la precisión, integridad o idoneidad de estos materiales para ningún propósito particular. 
   
3. El autor no se hace responsable de ningún perjuicio, incluyendo, pero no limitado a, daños directos, indirectos, incidentales, consecuenciales o especiales derivados del uso o la imposibilidad de uso de los materiales de este repositorio o su documentación asociada, incluso si los posibles daños fueron anticipados.

4. Al utilizar estos materiales, usted reconoce y asume todos los riesgos asociados con su aplicación. Además, acepta que el autor no puede ser considerado responsable de problemas o consecuencias derivadas de su uso.

</details> 

---

<h3 align="center"> 
💖 Apoya el proyecto 
</h3>

<p align="center"> 
Si este proyecto le fue útil, puede valorarlo dándole una estrella.:star2: 
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
Las donaciones son muy bienvenidas, por pequeñas que sean, y muchas gracias. 😌 
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
  <sub> Gracias por su interés en el proyecto y por su apoyo 💙 </sub>
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
    <summary>⚙️ Descripción expandida</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Desactivación de plugins

<details> 
    <summary>⚙️ Descripción expandida</summary>

- **SteamSockets:** El driver del plugin SteamSockets es necesario para el funcionamiento de Steam, pero dentro del marco del Advanced Sessions Plugin debe ser desactivado.

</details> 



## 📊 Funciones || Características

<details> 
    <summary>⚙️ Descripción expandida</summary>



</details>


# Project - Maps & Modes

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Propósito de la sección

La sección **Project - Maps & Modes** define los puntos clave de entrada del flujo de juego y la arquitectura del proyecto. Aquí se configura:

---

- qué `GameMode` se utiliza por defecto;
- qué mapas (maps) se cargan al iniciar el editor, el juego y el servidor;
- qué clases base se aplican (`Pawn`, `Controller`, `HUD`, etc.);
- cómo reemplazar automáticamente `GameMode` dependiendo del mapa o su prefijo.

De hecho, esta es la **puerta de entrada a la arquitectura del flujo de juego**.

---

# Default Modes

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Default GameMode.png"/>
</div>


## Default GameMode

**Default GameMode** - es el `GameMode` que será utilizado:

- si el mapa no redefine `GameMode`;
- si `GameMode` no está especificado a través de parámetros URL;
- si no funcionan los prefijos o alias.


#### Uso típico

- `GM_Menu` - menú principal
- `GM_Gameplay` - juego principal
- `GM_Lobby` - lobby multijugador

#### Importante

- `GameMode` existe **solo en el servidor** (o en un jugador único, como server-authority).
- Los clientes obtienen datos a través de `GameState`.

---

## Selected GameMode

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

Este bloque define un conjunto de clases para el `GameMode` seleccionado (en este caso `GM_Menu`).

---

### Default Pawn Class

Define qué `Pawn` será generado automáticamente para el jugador.

Ejemplos:

- `Pawn` - básico para el menú
- `Character` - si se requiere un personaje completo
- `SpectatorPawn` - si el jugador no debe controlar un cuerpo

Para menús:

- frecuentemente se usa un `Pawn` vacío o lógica mínima sin control.

---

### HUD Class

Clase `HUD` (obsoleta, pero aún soportada).

Utilizada si:

- la interfaz gráfica se dibuja mediante `DrawHUD`;
- se aplica lógica antigua del HUD.

Práctica moderna:

- `HUD` vacío;
- la interfaz gráfica se crea mediante **UMG** en `PlayerController`.

Para menús es aceptable usar un `HUD_Menu`.

---

### Player Controller Class

Una de las clases clave de la arquitectura.

Responsable de:

- entrada (`Input`);
- creación de la interfaz gráfica;
- control de la cámara;
- alternar modos de entrada (UI / Game).

Ejemplos:

**En menús**
- `PC_Menu`
- `Show Mouse Cursor` habilitado
- `Set Input Mode UI Only`

**En juego**
- `PC_Gameplay`
- `Game Only` o `Game and UI`

---

### Game State Class

`GameState` existe **en el servidor y en los clientes**.

Se utiliza para:

- temporizadores;
- la etapa actual del partido;
- el estado global del juego.

Ejemplo:

- `Server_GameState`

Incluso en un solo jugador, se recomienda almacenar datos en `GameState` en lugar de `GameMode`.

---

### Player State Class

`PlayerState` existe para cada jugador.

Almacena:

- puntajes;
- nombre;
- equipo;
- habilidades;
- estadísticas.

Aplicación:

- en multijugador, es obligatorio;
- en un solo jugador, es recomendado.

---

### Spectator Class

`Pawn` utilizado:

- al morir;
- al observar;
- al no tener un `Pawn` activo.

Por defecto, `SpectatorPawn` es una elección adecuada.

---

## Advanced (GameMode)

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced.png"/>
</div>

### Global Default Server Game Mode

Se utiliza **solo para servidores dedicados**.

Si se configura:

- el servidor siempre usará este `GameMode`;
- independientemente del mapa.

Normalmente:

- `None` - opción estándar;
- aplicada en compilaciones de servidor.

---

### Game Mode Map Prefixes

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>

Permite asignar automáticamente un `GameMode` según el prefijo del mapa.

Ejemplo:

- `MP_` -> `GM_Multiplayer`
- `SP_` -> `GM_Singleplayer`
- `MENU_` -> `GM_Menu`

#### Aplicación práctica

- una sola compilación;
- diferentes modos sin configuraciones manuales de mapas.

Extremadamente útil en proyectos medianos y grandes.

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
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Aliases.png"/>
</div>

Permite usar alias cortos para `GameMode`. Ideal cuando los mapas son los mismos, pero las reglas del juego son específicas.

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

Modos Lobby y de servicio:

- `"MENU"`  -> `GM_Menu`
- `"LOBBY"` -> `GM_Lobby`
- `"ENTRY"` -> `GM_Entry`

Modo individual:

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
### A través de la consola o línea de comandos

```ini
open Lvl_Arena?game=DM
```

Unreal Engine busca `DM` en `Game Mode Class Aliases`, ignora el `Default GameMode` y lo reemplaza por `GM_Deathmatch`,


### A través de Server Startup

```ini
UEGameServer.exe Lvl_Map?game=TDM?listen
```

### Muy útil para:

- servidores dedicados,
- CI/CD,
- pruebas automáticas.

---

### Cuando NO son necesarios los alias

Los alias no son esenciales si utilizas:

- `Map Override` en World Settings,
- `Game Mode Map Prefixes`,
- un `Default GameMode` fijado.

> En proyectos pequeños singleplayer, los alias rara vez se usan.


### Esquema recomendado para un proyecto real

Usar los tres mecanismos según corresponda:
|Mecanismo|Propósito|
|:---------:|:---------|
| Default GameMode | Fallback seguro |
| Map Override | Comportamiento explícito del mapa |
| Prefixes | Mapas masivos |
| Aliases | CLI, servidor, automatización |

---






## Default Maps

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/Default Maps.png"/>
</div>

### Editor Startup Map

El mapa que:

- automáticamente se abre al iniciar el editor.

Recomendación:

- mapa ligero;
- no la escena principal del juego;
- a menudo uno de prueba o menú.

---

### Editor Template Map Overrides

Uso raro.

Propósito:

- sobrescribir mapas de plantilla (template maps);
- pertinente para plantillas personalizadas.

En la mayoría de los proyectos no se utiliza.

---

### Game Default Map

El mapa que:

- se carga al iniciar el juego;
- utilizado en el packaged build.

Usualmente:

- el menú principal;
- o la primera escena del juego.

---

## Advanced (Maps)

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes - Default GameMode" src="../media/Tutorial/Article_1/Default Maps - Advanced.png"/>
</div>

### Local Map Options

Permite definir parámetros por defecto en la URL.

Ejemplo:

```ini
?listen?game=GM_Gameplay
```

Usado para:

- pruebas;
- servidores locales;
- parámetros automáticos de inicio.

---

### Transition Map

Mapa que:

- se carga temporalmente durante los cambios de nivel (Seamless Travel).

Uso multijugador:

- para evitar parones;
- para transiciones suaves entre niveles.

En un solo jugador, usualmente no es necesario.

---

### Server Default Map

El mapa que:

- se carga al iniciar un servidor dedicado.

Por lo general:

- `Entry`;
- o `Lvl_Lobby`.

Importante:

- no afecta al cliente;
- solo aplica en compilaciones de servidor.

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
- **Gameplay Maps**      -> `GM_Gameplay` (vía Override o Prefix)

Esta estructura asegura una clara separación entre menú, gameplay y lógica de servidor, además de simplificar la escalabilidad del proyecto.





* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 


<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

# Create Session 

<h1 align="center"> 
Create Session con configuración previa
</h1>

<details> 
    <summary> ⚙️ Descripción expandida </summary>

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
Find Session con configuración previa
</h1>

<details> 
    <summary> ⚙️ Descripción expandida </summary>

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
    <summary> ⚙️ Descripción expandida </summary>

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

# Comprobaciones

<h1 align="center"> 
Is Server -> Is Standalone -> Set Text
</h1>

<details> 
    <summary> ⚙️ Descripción expandida </summary>

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
Has Online Subsystem qué subsistema está activo
</h1>

<details> 
    <summary> ⚙️ Descripción expandida </summary>

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











<h1 align="center"> 📜 Licencia </h1>
<p align="center">
  <strong> Este proyecto se encuentra bajo la </strong> 
  <a href="/LICENSE">Apache License</a> 
</p>

---

<h2 align="center"> 
Documentación - revísela 
</h2>

<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">Inglés</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chino</a> |
  <strong><-------</strong>
</p>


<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">Inglés</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chino</a> |
  <strong><-------</strong>
</p>
