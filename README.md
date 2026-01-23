# LumenPnP Paste Extruder

This repository contains the source for the paste extruder toolhead for the LumenPnP.

![paste extrusion](./img/hero-paste.gif)

**This is an experimental product. The hardware is stable, but using the extruder will require tuning for your material and application.**

This extruder head is designed for solder paste and ink dispensing applications. It quickly and easily replaces the right toolhead on any version LumenPnP. It has been used to apply conductive ink and Loctite GC-10 solder paste onto PCBs.

Controlling this toolhead is currently done using [paste.opulo.io](paste.opulo.io), a web-based utility for automatically dispensing solder paste onto PCB pads based on your gerber files.

You can also control the paste extruder using `leash`, a python libary for interfacing with the LumenPnP, which can be found [here](https://github.com/opulo-inc/leash). There's an example script in `./sw/extrude/extrude.py` that you can use as a starting point for your own application.

The source CAD for the extruder was originally designed as a replacement left nozzle. However, the toolhead works much better when replacing the right nozzle. If printing yourself, ensure that you're respecting the mirror operation in the `extruder-base` and `cartridge-clamp` FDM parts. All other models can be used normally.

## Parts

| Item | Quantity |
| ---- | -------- |
| [M3 Nut](https://www.mcmaster.com/90591A250/) | 1 |
| [M3 Threaded Rod](https://www.mcmaster.com/94595A215/) | 1 |
| [Nema 11 Stepper Motor (The higher current rating the better)](https://www.amazon.com/s?k=nema+11+stepper+motor) | 1 |
| [M2.5x5mm Socket Head Bolt](https://www.mcmaster.com/91290A100/) | 4 |
| [M3 Square Nut](https://www.mcmaster.com/97259A101/) | 1 |
| [M3x20mm Socket Head Bolt](https://www.mcmaster.com/91290A123/) | 1 |
| [3ml Luer Lock Syringe](https://www.mcmaster.com/7510A42/) | 1 |
| [Luer Lock Tip (size depends on application)](https://www.mcmaster.com/products/needles/fitting-connection~luer-lock/dispensing-tips-with-luer-lock-connection/tip-type~tapered/) | 1 |

## Install

Installation and setup instructions can be found in this video:

[![](https://img.youtube.com/vi/N_p62_QUoKI/0.jpg)](https://youtu.be/N_p62_QUoKI)

## Help

Feel free to hop in the [LumenPnP Discord Server](https://discordapp.com/invite/TCwy6De ) to help debug and troubleshoot using the extruder head. Also, please feel free to add Github Issues on this repository if you discover any problems.
