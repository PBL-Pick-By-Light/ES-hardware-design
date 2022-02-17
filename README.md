# Hardware Design

## Introduction

Welcome to the hardware design repository of the Pick-by-Light projekt!

![Our implemented PBL system render](Documentation/Users%20Guide/Render/container.png)

![Our implemented PBL system real](Documentation/Users%20Guide/pictures/PBLDemoGif.gif)

The PBL project is designed to upgrade a small parts container with a microcontroller and LEDs.
In this repository you will find everything physically related to build the PBL, all software can be found in the other repositories.

In our implementation we installed the LEDs and the microcontroller via 3D printed parts and added acrylic glass sheets underneath each drawer to relay the emitted light of the LEDs. All necessary parts, further instructions to replicate our implementation and technical specs can be found in the [docs subfolder][docslink], also available as [PDF][UserGuidePDF] to print.

The PBL project is an open source project and we highly encourage you to modify and adjust everything to fit your needs. You can devise your own holding mechanisms and attachement of LEDs. The only necessity to work properly with the firmware is the usage of Adafruit adressable LEDs and an ESP32 microcontroller.

## Index

* [docs][docslink]
 - [Parts Listing](docs/PartsListingREADME.md)
 - [Technical Specs](docs/TechnicalSpecsREADME.md)
 - [Assembly and Installation](docs/AssemblyAndInstallationREADME.md)
* [Documentation][documentationlink]
* [Fusion360][fusionlink]
* [Master3DFiles][3dlink]

docs: all documentation about used hardware, which spare parts container we used and how to install everything to it as Readme files

Documentation: all files regarding documentation and complementing the users guide

Fusion360: Fusion360 project files to edit yourself to fit on different spare parts containers

Master3DFiles: all .stl and .obj files to put on a 3D printer


[docslink]:docs
[documentationlink]:Documentation
[fusionlink]:Fusion360
[3dlink]:Master3DFiles
[UserGuidePDF]:Documentation/PBL%20Users%20Guide.pdf