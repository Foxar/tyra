[![Contributors][contributors-shield]][contributors-url]
[![MIT License][license-shield]][license-url]
[![Discord](https://img.shields.io/badge/discord-Tyra-brightgreen?logo=discord)](https://discord.gg/NhhTmg3Gm5)
[![Discord](https://img.shields.io/badge/discord-PS2--Scene-brightgreen?logo=discord)](https://discord.gg/7dCr6ThSN5)

<br />
<p align="center">
  <a href="https://github.com/h4570/tyra">
    <img src="http://apgcglz.cluster028.hosting.ovh.net/tyra/github-splash.png" alt="Logo" width="100%" height="auto">
  </a>

  <h3 align="center">Tyra - alpha 1.31.2</h3>

  <p align="center">
    Open source game engine for PlayStation 2™
    <br />
    <a href="https://github.com/h4570/tyra/tree/master/src/samples/dolphin"><strong>Dolphin sample »</strong></a>
    &nbsp;
    <a href="https://github.com/h4570/tyra/tree/master/src/samples/floors"><strong>Floors sample »</strong></a>
    <br />
    <br />
    <a href="https://github.com/h4570/tyra/issues">Report Bug</a>
    ·
    <a href="https://github.com/h4570/tyra/issues">Request Feature</a>
  </p>
</p>  

[![Stargazers repo roster for h4570/tyra](https://reporoster.com/stars/h4570/tyra)](https://github.com/h4570/tyra/stargazers)

## Table of Contents  

* [About the Project](#about-the-project) 
  * [Samples](#samples) 
  * [About project](#about-project) 
  * [Tyra features](#tyra-features) 
  * [Branches](#branches) 
* [Getting Started](#getting-started) 
  * [Installation](#installation) 
  * [Prerequisites](#prerequisites) 
* [Roadmap](#roadmap) 
* [Contributing](#contributing) 
* [License](#license) 
* [Built With](#built-with) 
* [Acronyms](#acronyms) 
* [Thanks](#thanks) 

## About the Project  

<img src="http://apgcglz.cluster028.hosting.ovh.net/tyra/1.31.2/tyra.gif" alt="Sample code" width="600" height="auto">  
<img src="http://apgcglz.cluster028.hosting.ovh.net/tyra/1.31.2/samples/dolphin/dolphin.gif " alt="Sample game" width="500" height="auto">  

### Samples
* [Dolphin](https://github.com/h4570/tyra/tree/master/src/samples/dolphin) 
* [Floors](https://github.com/h4570/tyra/tree/master/src/samples/floors) 
* [Cube](https://github.com/h4570/tyra/tree/master/src/samples/cube) 
  
### About the project
Goal of Tyra project is to provide simple API for PS2 game creation, so you can just run PS2 emulator, grab .obj file, and put it into live in a seconds. Project is on alpha stage, so keep in mind that there are many things to be done and to fix.
 
YouTube tutorials soon!  
  
**Why Tyra is needed?** Raw PS2 development can be a big challenge. PS2 it's pretty low-level and there are a lot of stuff that you must do from scratch.  
Tyra takes care for you, and rendering, coprocessors communication, synchronization and many more low-level stuff is already done.

### Tyra features
* 3D support - VU1 "Path 1 rendering"  
* 2D support - PNG & BMP
* Frustum culling, backface culling  
* OpenGL adaptions: Perspective projection, lookAt camera  
* Texture support - .bmp and png  
* Mesh loaders: ".obj", ".dff" (RenderWare, GTA:SA) and ".md2" (Quake II) 
* Threading support 
* Animation support for obj and md2
* Audio support - .wav and .adpcm 
* Pad support 

### Branches
* Master - monthly releases - tested on PS2 & PCSX2.
* Develop - daily builds - can be unstable.

## Getting Started  

### Installation [![Discord](https://img.shields.io/badge/discord-Tyra-brightgreen?logo=discord)](https://discord.gg/NhhTmg3Gm5)  
In our Discord channel, there is detailed tutorial which will help you with setting up the all environment - starting from installing dependencies and ending on emulator setup or intellisense.  

### Prerequisites 

* PS2 DEV environment - [PS2DEV](https://github.com/ps2dev/ps2dev)  
* At least #e8e9edb PS2SDK (06.02.2021) - [PS2SDK](https://github.com/ps2dev/ps2sdk) 
* PS2 Emulator. For example [PCSX2](https://pcsx2.net/) 

## Extra info 
* BMP loader needs some polishing so be sure that you exporting BMP with 24bit: RGB888 and without information about colors. 
* If you want to run .elf in PCSX2, be sure that you have version >=1.6 and **Host access** enabled in PCSX2 configuration file.  
* If you want to use your own .obj file, please check "triangulate faces" in blender. PS2 is supporting only triangle primitive type.  

## Roadmap  

### Roadmap for next master release:  
[Next release roadmap](https://github.com/h4570/tyra/projects/4)  

See the [open issues](https://github.com/h4570/tyra/issues) for a list of proposed features (and known issues). 

## Contributing 

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**. 

1. Fork the Project 
2. Create your Feature Branch (`git checkout -b feature/amazing-feature`)  
3. Commit your Changes (`git commit -m 'Add some amazing-feature'`)  
4. Push to the Branch (`git push origin feature/amazing-feature`)  
5. Open a Pull Request  

## License  

Distributed under the Apache License 2.0 License. See `LICENSE` for more information. 

## Built With  

* [PS2SDK](https://github.com/ps2dev/ps2sdk)  

### Acronyms 
* EE (Emotion Engine) - whole set of processors and subsystems that make up the PlayStation 2 
* GS (Graphic synthesizer) - configurable rasterizer and texture mapper. Has only 2MB~ memory for textures, but for the opposite have very high transfer rate, so you can switch textures in the blink 
* VU0 - programmable (ASM) vector processor that is accessed by inline assembly code injected into C program.  
* VU1 - programmable (ASM) vector processor, which is similar to vertex shader. Accessed via DMA.  
* IOP - I/O processor which enables access to peripheral devices, such the game controller  

## Thanks  

Without these guys, everything would be harder:
* Dr Henry Fortuna - for code sources
* Rick Gaiser - for help and new GCC!
* Lukasz D.K. - for huge archive of PS2 stuff
* Guilherme Lampert - for code sources
* Jesper Svennevid, Daniel Collin - for openvcl's code samples
* Whole PS2DEV team
* Manieq - for nice splash screens!
* And so many other guys. Thanks!

Project Link: [https://github.com/h4570/tyra](https://github.com/h4570/tyra)  
Sandro Sobczyński - sandro.sobczynski@gmail.com  
[![LinkedIn][linkedin-shield]](https://linkedin.com/in/sandro-sobczyński-28820b15a)  
  
<br />
<a href="https://github.com/h4570/tyra">
  <img src="http://apgcglz.cluster028.hosting.ovh.net/tyra/github-splash2.png" alt="Logo" width="100%" height="auto">
</a>

[contributors-shield]: https://img.shields.io/github/contributors/h4570/tyra.svg?style=flat-square  
[contributors-url]: https://github.com/h4570/tyra/graphs/contributors 
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555  
[license-shield]: https://img.shields.io/github/license/h4570/tyra.svg?style=flat-square  
[license-url]: https://github.com/h4570/tyra/blob/master/LICENSE  
