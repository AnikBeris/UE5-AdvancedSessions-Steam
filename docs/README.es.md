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
> 💡 Este material está orientado a usuarios avanzados.
</h2>


* * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * 



<h2 align="center">
⚠️ Exención de responsabilidad ⚠️
</h2>

<p align="center">
  El autor no se responsabiliza de las posibles consecuencias del uso de este proyecto.<br>
  Úselo bajo su propio riesgo.
</p>

<details align="center"> 
    <summary>⚠️texto completo⚠️</summary>
    
Utilice los recursos de este repositorio bajo su propia responsabilidad.

1. Al usar los materiales de este repositorio, usted acepta automáticamente los términos y condiciones de la licencia asociada.

2. El autor no ofrece ninguna garantía, explícita o implícita, respecto a la exactitud, integridad o adecuación de estos materiales para fines específicos.
   
3. El autor no será responsable de ninguna pérdida, incluidos, entre otros, daños directos, indirectos, incidentales o especiales resultantes del uso o la incapacidad de usar los materiales de este repositorio o la documentación asociada, incluso si se informó con antelación sobre la posibilidad de dichos daños.

4. Al usar estos materiales, usted reconoce y asume todos los riesgos asociados con su aplicación. Además, acepta que el autor no será responsable de ningún problema o consecuencia derivada de su uso.

</details> 

---

<h3 align="center"> 
💖 Apoya el proyecto 
</h3>

<p align="center"> 
Si este proyecto le ha resultado útil, puede valorarlo marcándolo con una estrella.:star2: 
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
  <sub> Gracias por su interés en el proyecto y su apoyo 💙 </sub>
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
    <summary>⚙️ Expandir descripción</summary>

- **Advanced Sessions Plugin:** 
- **Steam:** 

</details> 



## 📊 Desactivación de plugins

<details> 
    <summary>⚙️ Expandir descripción</summary>

- **SteamSockets:** El controlador del plugin SteamSockets es necesario para que funcione Steam, pero en el marco de Advanced Sessions Plugin debe desactivarse.

</details> 



## 📊 Funciones || Características

<details> 
    <summary>⚙️ Expandir descripción</summary>



</details>


# Project - Maps & Modes

<div align="center">
  <img style="width: 90%; height: auto;" alt="Project-Maps&Modes" src="../media/Tutorial/Article_1/Project-Maps&Modes.png"/>
</div>

## Propósito de esta sección

La sección **Project - Maps & Modes** define los puntos de entrada clave del flujo de juego y la arquitectura del proyecto. Aquí se configura:

---

- qué `GameMode` se usa por defecto;
- qué mapas (maps) se cargan al iniciar el editor, el juego y el servidor;
- qué clases base se aplican (`Pawn`, `Controller`, `HUD`, etc.);
- cómo cambiar automáticamente el `GameMode` dependiendo del mapa o su prefijo.

De hecho, esta es **la entrada principal a la arquitectura del flujo del juego**.

---


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
