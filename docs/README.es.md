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
[![GitHub Stars](https://img.shields.io/github/stars/AnikBeris?style=flat&logo=github&label=Estrellas&color=orange)](https://github.com/AnikBeris)

</div>

<div align="center">
  <img src="../media/image0.gif" alt="SPACER" width="90%">
</div>


<h1 align="center"> 
Información útil sobre el desarrollo de un proyecto en Unreal Engine 5 utilizando el plugin AdvancedSessions-Steam
</h1>

<h2 align="center">
> 💡 El material está orientado para usuarios con conocimientos previos.
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
    <summary>⚠️texto completo⚠️</summary>
    
Utilice los materiales de este repositorio bajo su propio riesgo.

1. Al usar los materiales de este repositorio, usted acepta automáticamente los términos del acuerdo de licencia relacionado con ellos.

2. El autor no ofrece ninguna garantía, ya sea implícita o explícita, sobre la precisión, integridad o idoneidad de estos materiales para cualquier propósito específico.
   
3. El autor no se hace responsable de ningún daño, incluidos, entre otros, daños directos, indirectos, incidentales, consecuenciales o especiales, que resulten del uso o la imposibilidad de usar los materiales de este repositorio o la documentación asociada, incluso si se le ha informado previamente de la posibilidad de tales daños.

4. Al usar estos materiales de este repositorio, usted acepta y asume todos los riesgos asociados con su aplicación. Además, usted acepta que el autor no puede ser considerado responsable de ningún problema o consecuencia que surja como resultado de su uso.

</details> 

---

<h3 align="center"> 
💖 Apoya el proyecto 
</h3>

<p align="center"> 
Si este proyecto te resultó útil, puedes valorarlo con una estrellita.:star2: 
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
Las donaciones son muy bienvenidas, por pequeñas que sean, y de corazón, ¡muchas gracias! 😌 
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
  <sub> Gracias por tu atención al proyecto y por tu apoyo 💙 </sub>
</p>

---

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



## 📚 Índice

- [Introducción](#-introducción)




## 🔗 Enlaces útiles



* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-índice"> ⬆️ Subir arriba </a> 
</h2>

<h1 align="center"> 
Requisitos técnicos
</h1>



## 📊 Plugins instalados

<details> 
    <summary>⚙️ Desplegar descripción</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Desactivación de plugins

<details> 
    <summary>⚙️ Desplegar descripción</summary>

- **SteamSockets:** El controlador del plugin SteamSockets es necesario para el funcionamiento de Steam pero, en el marco de Advanced Sessions Plugin, debe desactivarse.

</details> 



## 📊 Funciones || Características

<details> 
    <summary>⚙️ Desplegar descripción</summary>



</details>


<h2 align="center">
  <a href="#-índice">⬆️ Subir arriba</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center"> 
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Propósito de la sección

La sección **Project - Maps & Modes** define puntos clave de entrada en el flujo del juego y la arquitectura del proyecto. Aquí se configura:

---

- qué `GameMode` se utiliza por defecto;
- qué mapas (maps) se cargan al iniciar el editor, el juego y el servidor;
- qué clases base se aplican (`Pawn`, `Controller`, `HUD`, etc.);
- cómo reemplazar automáticamente el `GameMode` dependiendo del mapa o su prefijo.

De hecho, este es el **punto de entrada a la arquitectura del flujo del juego**.

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 




<h2 align="center">
  <a href="#-índice">⬆️ Subir arriba</a> 
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

**Default GameMode** - es el `GameMode` que se utilizará:

- si el nivel no redefine el `GameMode`;
- si el `GameMode` no está especificado a través de parámetros URL;
- si no funcionan los prefijos o alias.

#### Aplicación típica

- `GM_Menu` - menú principal
- `GM_Gameplay` - juego principal
- `GM_Lobby` - lobby multijugador

#### Importante

- `GameMode` existe **solo en el servidor** (o en el jugador único, como server-authority).
- Los clientes reciben datos a través de `GameState`.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-índice">⬆️ Subir arriba</a> 
</h2>

###### # Selected GameMode

<h1 align="center"> 
Selected GameMode
</h1>

<div align="center">
  <img style="width: 90%; height: auto;" alt="DefaultModes -Selected GameMode" src="../media/Tutorial/Article_1/DefaultModes -Selected GameMode.png"/>
</div>

**Selected GameMode** - Este bloque define un conjunto de clases para el `GameMode` seleccionado (en este caso `GM_Menu`).

<details> 
    <summary> ⚙️ Desplegar descripción </summary>

---

### Default Pawn Class

Determina qué `Pawn` será generado automáticamente para el jugador.

Ejemplos:

- `Pawn` - un placeholder para el menú
- `Character` - si se necesita un personaje completo
- `SpectatorPawn` - si el jugador no debe controlar un cuerpo

Para el menú:

- se usa a menudo un `Pawn` vacío o lógica mínima sin control.

---

### HUD Class

Clase `HUD` (obsoleta, pero todavía admitida).

Se utiliza si:

- la interfaz de usuario se dibuja a través de `DrawHUD`;
- se aplica la lógica antigua de HUD.

Práctica moderna:

- `HUD` vacío;
- la interfaz de usuario se crea mediante **UMG** en `PlayerController`.

Para el menú es aceptable usar `HUD_Menu`.

---

### Player Controller Class

Una de las clases clave de la arquitectura.

Es responsable de:

- entrada (`Input`);
- creación de UI;
- control de cámara;
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

`GameState` existe **en el servidor y los clientes**.

Se utiliza para:

- temporizadores;
- estado actual del partido;
- estado global del juego.

Ejemplo:

- `Server_GameState`

Incluso en jugador único se recomienda almacenar los datos en `GameState` y no en `GameMode`.

---

### Player State Class

`PlayerState` existe para cada jugador.

Almacena:

- puntos;
- nombre;
- equipo;
- habilidades;
- estadísticas.

Aplicación:

- en multijugador - obligatorio;
- en jugador único - recomendable.

---

### Spectator Class

`Pawn` que se utiliza:

- al morir;
- al observar;
- en ausencia de un `Pawn` activo.

Por defecto, `SpectatorPawn` es una elección correcta.

</details> 

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
  <a href="#-índice">⬆️ Subir arriba</a> 
</h2>

