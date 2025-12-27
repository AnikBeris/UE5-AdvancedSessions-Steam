<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Español</a> |
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
Información útil sobre el desarrollo de proyectos en Unreal Engine 5 utilizando el plugin AdvancedSessions-Steam
</h1>

<h2 align="center">
> 💡 El material está orientado a usuarios experimentados.
</h2>

* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 

<h2 align="center">
⚠️ Descargo de responsabilidad ⚠️
</h2>

<p align="center">
  El autor no se responsabiliza de las posibles consecuencias derivadas del uso de este proyecto.<br>
  Úselo bajo su propia responsabilidad.
</p>

<details align="center"> 
    <summary>⚠️texto completo⚠️</summary>
    
Use los materiales de este repositorio bajo su propio riesgo.

1. Al utilizar los materiales de este repositorio, aceptas automáticamente los términos del acuerdo de licencia asociado.

2. El autor no ofrece ninguna garantía, expresa o implícita, sobre la precisión, integridad o idoneidad de estos materiales para ningún propósito específico.
   
3. El autor no se hace responsable de ninguna pérdida, incluyendo, entre otras, pérdidas directas, indirectas, incidentales o especiales que deriven del uso o de la imposibilidad de usar los materiales de este repositorio o su documentación asociada, incluso si se había informado previamente de la posibilidad de tales pérdidas.

4. Al usar los materiales de este repositorio, reconoces y aceptas todos los riesgos relacionados con su aplicación. Además, aceptas que el autor no podrá ser considerado responsable de ningún problema o consecuencia resultante de su uso.

</details> 

---

<h3 align="center">
💖 Apoya el proyecto 
</h3>

<p align="center"> 
Si este proyecto te ha sido útil, puedes mostrar tu apoyo dándole una estrella.:star2: 
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
Las donaciones son siempre bienvenidas, incluso las más pequeñas. Muchas gracias. 😌 
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
  <sub> Gracias por tu atención al proyecto y por tu apoyo 💙 </sub>
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
  <a href="#-contenido">⬆️ Arriba </a> 
</h2>

<h1 align="center">
Requisitos técnicos
</h1>

## 📊 Plugin instalado

<details> 
    <summary>⚙️ Mostrar descripción</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 

## 📊 Desactivación de plugins

<details> 
    <summary>⚙️ Mostrar descripción</summary>

- **SteamSockets:** El driver del plugin SteamSockets es necesario para Steam, pero para Advanced Sessions Plugin debe desactivarse.

</details> 

## 📊 Funciones || Características

<details> 
    <summary>⚙️ Mostrar descripción</summary>



</details>

<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

###### # Project - Maps & Modes

<h1 align="center">
Project - Maps & Modes
</h1>

<div align="center">
  <img style="width: 70%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Propósito de la sección

La sección **Project - Maps & Modes** define puntos clave de entrada al flujo de juego y la arquitectura del proyecto. Aquí se configura:

---

- qué `GameMode` se usa por defecto;
- qué mapas se cargan al iniciar el editor, el juego y el servidor;
- qué clases base se aplican (`Pawn`, `Controller`, `HUD`, etc.);
- cómo reemplazar automáticamente el `GameMode` dependiendo del mapa o su prefijo.

De hecho, es **el punto de entrada a la arquitectura del flujo de juego**.

<h2 align="center">
  <a href="#-contenido">⬆️ Arriba</a> 
</h2>

<h1 align="center"> 📜 Licencia </h1>
<p align="center">
  <strong> Este proyecto está bajo la </strong> 
  <a href="/LICENSE">Apache License</a> 
</p>

---

<h2 align="center"> 
Consulta la documentación 
</h2>

<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chinese</a> |
  <strong><-------</strong>
</p>

<p align="center">
  <strong>-------></strong>
  <a href="/README.md">Русский</a> |
  <a href="/docs/README.en.md">English</a> |
  <a href="/docs/README.es.md">Español</a> |
  <a href="/docs/README.zh.md">Chinese</a> |
  <strong><-------</strong>
</p>
