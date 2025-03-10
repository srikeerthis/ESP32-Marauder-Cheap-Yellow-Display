# ESP32-Marauder-Cheap-Yellow-Display

<p align="center">
  <img alt="Marauder logo" src="https://github.com/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display/blob/master/img/logo01.png" width="240">
</p>

<p align="center"> <img src="https://github.com/Fr4nkFletcher/Adafruit_WebSerial_ESPTool/actions/workflows/pages.yml/badge.svg" /> <img src="https://komarev.com/ghpvc/?username=Fr4nkFletcher&label=Views&color=0e75b6&style=flat" alt="Fr4nkFletcher" />
<img src="https://img.shields.io/github/issues/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display?style=flat-square" />
</p>

<div align="center">
  
  ## 🏴‍☠️ Update Highlights 09/28/24 — Flash previous Marauder versions 🏴‍☠️

</div>

- **For info on swapping to the ESP-WROOM-32U w/ built-in IPEX/U.FL connector for max range, click [here](https://github.com/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display/blob/master/AntennaModNew.md).**

- **For Evil Portal examples and instructions, click [here](https://github.com/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display/blob/master/evilportal/).**

- **For info on adding an external antenna, click [here](https://github.com/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display/blob/master/AntennaMod.md).**


## Web Flasher Instructions
-  **Use Chrome**

- **Visit:** [CYM-Web-Flasher](https://fr4nkfletcher.github.io/Adafruit_WebSerial_ESPTool/)

- **Click Connect** and select **Model** and **Version**. Click **Program** to start the flashing process.

<p align="center">
  <img src="https://github.com/Fr4nkFletcher/Adafruit_WebSerial_ESPTool/blob/main/assets/sc002.png?raw=true" alt="CYM Web Flasher Screenshot" width="100%" style="max-width:800px; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

  **If you have issues with the web flasher, try unplugging and restarting your CYD, then hold RST --> tap BOOT --> release RST.
  You should get a blank screen. Refresh the webflasher and then click Connect to begin the process.**
  
  **If issues still persist, hold BOOT while clicking Connect**

   For more info on the webflasher visit ---> https://github.com/Fr4nkFletcher/Adafruit_WebSerial_ESPTool
 
</p>



## Compatibility

Successfully tested on both of these devices:
- [Module 1](https://amazon.com/dp/B0BVFXR313)
- [Module 2](https://amazon.com/dp/B0CLR7MQ91)

No hardware modifications required thanks to integration with **@ggaljoen's** [TFT_eSPI](https://github.com/ggaljoen/TFT_eSPI) fork.

- **GPS Functionality**: 🛰 GPS is [enabled](screenshots/gps5.jpg) and fully operational through the 4-pin connector located near the MicroUSB port of the CYD module. [Check here](https://github.com/justcallmekoko/ESP32Marauder/wiki/gps-modification) for details on supported GPS hardware.

**GPS Pinout:**

| GPS    |  ->  | CYD    |
|--------|------|--------|
| VCC    |  ->  | VIN    |
| GND    |  ->  | GND    |
| TX     |  ->  | TX     |
| RX     |  ->  | TX     |

## Setup

Add necessary libraries to your Arduino libraries folder. Configure your Arduino environment as detailed in the [ESP32 Marauder Arduino IDE Setup Guide](https://github.com/justcallmekoko/ESP32Marauder/wiki/arduino-ide-setup).

Ensure the upload speed is set to `115200` in Arduino IDE (tested with version 1.8.19).

**If you're having issues or want to do everything yourself, [check Smoochiee's tutorial](https://github.com/smoochiee/MARAUDER-FOR-CYD---CHEAP-YELLOW-DISPLAY) for an in-depth walkthrough of the port.**

## Acknowledgments

A big shoutout to the creators and supporters of the [ESP32 Cheap Yellow Display](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display) project and the community Discord, especially **@cod5fgzj**, [**smoochiee**](https://github.com/smoochiee), [**ggaljoen**](https://github.com/ggaljoen), and [**ATOMNFT**](https://github.com/ATOMNFT). And of course [**JustCallMeKoko**](https://github.com/justcallmekoko) for the foundational work on the [ESP32Marauder](https://github.com/justcallmekoko/ESP32Marauder).

<p align="center">
  <img src="https://github.com/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display/blob/master/screenshots/2.gif" alt="Demo 1">
  <img src="https://github.com/Fr4nkFletcher/ESP32-Marauder-Cheap-Yellow-Display/blob/master/screenshots/swift2.gif" alt="Demo 2">
</p>

