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
    <img alt="Logo del Proyecto" src="../media/logo-light.png" width="512" height="auto">
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
> 💡 El material está orientado a usuarios con experiencia.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Descargo de responsabilidad ⚠️
</h2>

<p align="center">
  El autor no se hace responsable de las posibles consecuencias del uso de este proyecto.<br>
  Úselo bajo su propio riesgo.
</p>

<details align="center"> 
    <summary>⚠️Texto completo⚠️</summary>
    
Utilice los materiales de este repositorio bajo su propio riesgo.

1. Al utilizar los materiales de este repositorio, usted acepta automáticamente los términos del acuerdo de licencia relacionados con él.

2. El autor no ofrece ninguna garantía, expresa o implícita, en cuanto a la precisión, la integridad o la idoneidad de estos materiales para fines específicos.
   
3. El autor no se hace responsable de ningún daño, incluyendo, entre otros, daños directos, indirectos, incidentales, consecuentes o especiales que surjan del uso o la imposibilidad de uso del material de este repositorio o de la documentación que lo acompaña, incluso si se advirtió previamente sobre la posibilidad de dichos daños.

4. Al utilizar este material del repositorio, usted acepta y asume todos los riesgos asociados con su aplicación. Además, acepta que el autor no podrá ser considerado responsable de posibles problemas o consecuencias resultantes de su uso.

</details> 

---

<h3 align="center"> 
💖 Apoya el proyecto 
</h3>

<p align="center"> 
Si este proyecto le ha resultado útil, puede mostrar su agradecimiento dándole una estrella.:star2: 
</p>

<p align="center">
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="Invítame un café">
  </a>
  <a href="https://pay.cloudtips.ru/p/7249ba98" target="_blank">
    <img src="../media/buymeacoffe.png" alt="Invítame un café">
  </a>
</p>



<h4 align="center"> 
Las donaciones son muy bienvenidas, sean pequeñas o grandes. Muchas gracias. 😌 
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
    <summary>⚙️ Desplegar descripción</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Desactivación de plugins

<details> 
    <summary>⚙️ Desplegar descripción</summary>

- **SteamSockets:** El controlador del plugin SteamSockets es necesario para el funcionamiento de Steam, pero con el plugin Advanced Sessions Plugin debe estar desactivado.

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

La sección **Project - Maps & Modes** define puntos clave de entrada en el flujo de juego y la arquitectura del proyecto. Aquí se configura:

---

- qué `GameMode` se usa por defecto;
- qué mapas (maps) se cargan al iniciar el editor, el juego y el servidor;
- qué clases base se aplican (`Pawn`, `Controller`, `HUD`, etc.);
- cómo cambiar automáticamente el `GameMode` dependiendo del mapa o su prefijo.

De hecho, este es el **punto de entrada en la arquitectura del flujo del juego**.

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
    <summary> ⚙️ Desplegar descripción </summary>

**Default GameMode** - Es el `GameMode` que se utilizará:

- si el nivel no sobreescribe el `GameMode`;
- si el `GameMode` no se especifica a través de parámetros de URL;
- si no funcionan los prefijos o alias.

#### Uso típico

- `GM_Menu` - menú principal
- `GM_Gameplay` - juego principal
- `GM_Lobby` - lobby multijugador

#### Importante

- El `GameMode` solo existe **en el servidor** (o en un jugador único como server-authority).
- Los clientes reciben datos a través de `GameState`.

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

**Selected GameMode** - Este bloque define las clases para el `GameMode` seleccionado (en este caso `GM_Menu`).

<details> 
    <summary> ⚙️ Desplegar descripción </summary>
---

### Default Pawn Class

Define qué `Pawn` será generado automáticamente para el jugador.

Ejemplos:

- `Pawn` - vacío para el menú
- `Character` - si se necesita un personaje completo
- `SpectatorPawn` - si el jugador no debe controlar un cuerpo

Para el menú:

- se suele usar un `Pawn` vacío o con lógica mínima sin control.

---

### HUD Class

Clase `HUD` (obsoleta, pero todavía compatible).

Se usa cuando:

- la UI se dibuja a través de `DrawHUD`;
- se aplica la lógica antigua del HUD.

Práctica moderna:

- `HUD` vacío;
- la UI se crea a través de **UMG** en `PlayerController`.

Para el menú, el uso de `HUD_Menu` es aceptable.

---

### Player Controller Class

Una de las clases clave de la arquitectura.

Responsable de:

- entrada (`Input`);
- creación de la UI;
- control de la cámara;
- cambio de modos de entrada (UI / Game).

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

`GameState` existe **en el servidor y en los clientes**.

Se usa para:

- temporizadores;
- la fase actual del partido;
- el estado global del juego.

Ejemplo:

- `Server_GameState`

Incluso en un jugador único, se recomienda almacenar datos en `GameState` en lugar de en `GameMode`.

---

### Player State Class

`PlayerState` existe para cada jugador.

Almacena:

- puntos;
- nombre;
- equipo;
- habilidades;
- estadísticas.

Uso:

- en multijugador - indispensable;
- en un jugador único - recomendable.

---

### Spectator Class

`Pawn` que se usa:

- en caso de muerte;
- al observar;
- cuando no hay un `Pawn` activo.

Por defecto, `SpectatorPawn` es una opción adecuada.

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
    <summary> ⚙️ Desplegar descripción </summary>

### Global Default Server Game Mode

- Solo se usa **en servidores dedicados**.

Si está configurado:

- el servidor siempre usará este `GameMode`;
- independientemente del mapa.

Normalmente:

- `None` - opción estándar;
- se aplica en compilaciones para servidores.

---

### Game Mode Map Prefixes

<div align="center">
  <img style="width: 80%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Prefixes" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Prefixes.png"/>
</div>

<div align="center">
  <img style="width: 40%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-PrefixesLevel" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-PrefixesLevel.png"/>
</div>


Permite asignar automáticamente `GameMode` según el prefijo del mapa.

Ejemplo:

- `MP_` -> `GM_Multiplayer`
- `SP_` -> `GM_Singleplayer`
- `MENU_` -> `GM_Menu`

#### Aplicación práctica

- una compilación;
- diferentes modos sin configuración manual de mapas.

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
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode-Advanced-Aliases" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode-Advanced-Aliases.png"/>
</div>

Permite usar alias cortos para el `GameMode`. Útil cuando hay mapas similares pero reglas específicas para el juego.

Ejemplo clásico de PvP:

- `"DM"`   -> `GM_Deathmatch`
- `"TDM"`  -> `GM_TeamDeathmatch`
- `"CTF"`  -> `GM_CaptureTheFlag`
- `"FFA"`  -> `GM_FreeForAll`
- `"KOTH"` -> `GM_KingOfTheHill`
- `"SD"`   -> `GM_SearchAndDestroy`

Ejemplo clásico de PvE:

- `"COOP"`  -> `GM_Coop`
- `"PVE"`   -> `GM_PvE`
- `"SURV"`  -> `GM_Survival`
- `"HORDE"` -> `GM_Horde`
- `"WAVES"` -> `GM_Waves`

Modos de lobby y de servicio:

- `"MENU"`  -> `GM_Menu`
- `"LOBBY"` -> `GM_Lobby`
- `"ENTRY"` -> `GM_Entry`

Modo solitario:

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


## Uso práctico
### A través de la consola o línea de comandos

```ini
open Lvl_Arena?game=DM
```

Unreal Engine busca `DM` en `Game Mode Class Aliases`, ignora el `Default GameMode` asignado y lo reemplaza por `GM_Deathmatch`,


### Durante Server Startup

```ini
UEGameServer.exe Lvl_Map?game=TDM?listen
```

### Muy práctico para:

- servidores dedicados,
- CI/CD,
- pruebas automáticas.

---

### Cuándo no se necesitan alias

Los alias no son imprescindibles si se utiliza:

- `Map Override` en World Settings,
- `Game Mode Map Prefixes`,
- valor fijo de `Default GameMode`.

> En proyectos pequeños para un jugador, a menudo no se utilizan alias.


### Esquema recomendado para un proyecto real

Usar los tres mecanismos con distintos propósitos:
|Mecanismo|Para qué sirve|
|:---------:|:---------|
| Default GameMode | Respaldo seguro |
| Map Override | Comportamiento explícito del mapa |
| Prefixes | Para mapas de manera masiva |
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
    <summary> ⚙️ Desplegar descripción </summary>


### Editor Startup Map

Mapa que:

- se abre automáticamente al iniciar el editor.

Recomendación:

- mapa liviano;
- no la escena principal del juego;
- frecuentemente de prueba o menú.

---

### Editor Template Map Overrides

Se utiliza poco.

Propósito:

- sobreescribir mapas de plantillas (template maps);
- relevante para plantillas personalizadas.

En la mayoría de los proyectos no se usa.

---

### Game Default Map

Mapa que:

- se carga al iniciar el juego;
- se usa en el build empaquetado.

Normalmente:

- menú principal;
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
    <summary> ⚙️ Desplegar descripción </summary>

### Local Map Options

Permite establecer parámetros de URL predeterminados.

Ejemplo:

```ini
?listen?game=GM_Gameplay
```

Se usa para:

- pruebas;
- servidores locales;
- parámetros automáticos al iniciar.

---

### Transition Map

Mapa que:

- se carga temporalmente al cambiar de niveles (Seamless Travel).

Se usa en multijugador:

- para evitar congelamientos;
- para una transición fluida entre niveles.

En un jugador único, normalmente no es necesario.

---

### Server Default Map

Mapa que:

- se carga al iniciar un servidor dedicado.

Normalmente:

- `Entry`;
- o `Lvl_Lobby`.

Importante:

- no afecta al cliente;
- solo se aplica en versiones de servidor.

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
- **Gameplay Maps**      -> `GM_Gameplay` (mediante Override o Prefijo)

Esta configuración asegura una separación clara entre el menú, el gameplay y la lógica del servidor, además de simplificar la escalabilidad del proyecto.

</details> 




* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 


<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Create Session 

<h1 align="center"> 
Crear sesión con configuración previa
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
Encontrar sesión con configuración previa
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
Has Online Subsystem cuál subsistema está activo
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
  <strong> Este proyecto está distribuido bajo la </strong> 
  <a href="/LICENSE">Licencia Apache</a> 
</p>

---

<h2 align="center"> 
Documentación, consúltela aquí 
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
