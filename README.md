Arduino core for ESP8266 WiFi chip
===========================================

# Quick links

- [Latest release documentation](https://arduino-esp8266.readthedocs.io/en/3.1.2/)
- [Current "git version" documentation](https://arduino-esp8266.readthedocs.io/en/latest/)
- [Install git version](https://arduino-esp8266.readthedocs.io/en/latest/installing.html#using-git-version) ([sources](doc/installing.rst#using-git-version))

# Arduino on ESP8266

This project brings support for the ESP8266 chip to the Arduino environment. It lets you write sketches, using familiar Arduino functions and libraries, and run them directly on ESP8266, with no external microcontroller required.

ESP8266 Arduino core comes with libraries to communicate over WiFi using TCP and UDP, set up HTTP, mDNS, SSDP, and DNS servers, do OTA updates, use a file system in flash memory, and work with SD cards, servos, SPI and I2C peripherals.

# Contents
- Installing options:
  - [Using Boards Manager](#installing-with-boards-manager)
  - [Using git version](#using-git-version)
  - [Using PlatformIO](#using-platformio)
  - [Building with make](#building-with-make)
- [Documentation](#documentation)
- [Issues and support](#issues-and-support)
- [Contributing](#contributing)  
- [License and credits](#license-and-credits)   

### Installing with Boards Manager

Starting with 1.6.4, Arduino allows installation of third-party platform packages using Boards Manager. We have packages available for Windows, Mac OS, and Linux (32 and 64 bit).

- [Download and install Arduino IDE 1.x or 2.x](https://www.arduino.cc/en/software)
- Start Arduino and open the Preferences window
- Enter `https://arduino.esp8266.com/stable/package_esp8266com_index.json` into the *File>Preferences>Additional Boards Manager URLs* field of the Arduino IDE. You can add multiple URLs, separating them with commas.
- Open Boards Manager from Tools > Board menu and install *esp8266* platform (and don't forget to select your ESP8266 board from Tools > Board menu after installation).

#### Latest release [![Latest release](https://img.shields.io/github/release/esp8266/Arduino.svg)](https://github.com/esp8266/Arduino/releases/latest/)
Boards manager link: `https://arduino.esp8266.com/stable/package_esp8266com_index.json`

Documentation: [https://arduino-esp8266.readthedocs.io/en/3.1.2/](https://arduino-esp8266.readthedocs.io/en/3.1.2/)

### Using git version

Also known as latest git or master branch.

- When using [Arduino IDE](https://www.arduino.cc/en/software), follow [our instructions here](https://arduino-esp8266.readthedocs.io/en/latest/installing.html#using-git-version).
- When using [PlatformIO](https://platformio.org/install), refer to [platformio/espressif8266 platform documentation](https://docs.platformio.org/en/stable/platforms/espressif8266.html#using-arduino-framework-with-staging-version).

### Using PlatformIO

[PlatformIO](https://platformio.org?utm_source=arduino-esp8266) is an open source ecosystem for IoT
development with a cross-platform build system, a library manager, and full support
for Espressif (ESP8266) development. It works on the following popular host operating systems: macOS, Windows,
Linux 32/64, and Linux ARM (like Raspberry Pi, BeagleBone, CubieBoard).

- [What is PlatformIO?](https://docs.platformio.org/en/latest/what-is-platformio.html?utm_source=arduino-esp8266)
- [PlatformIO IDE](https://platformio.org/platformio-ide?utm_source=arduino-esp8266)
- [PlatformIO Core](https://docs.platformio.org/en/latest/core.html?utm_source=arduino-esp8266) (command line tool)
- [Advanced usage](https://docs.platformio.org/en/latest/platforms/espressif8266.html?utm_source=arduino-esp8266) -
  custom settings, uploading to SPIFFS, Over-the-Air (OTA), staging version
- [Integration with Cloud and Standalone IDEs](https://docs.platformio.org/en/latest/ide.html?utm_source=arduino-esp8266) -
  Cloud9, Codeanywhere, Eclipse Che (Codenvy), Atom, CLion, Eclipse, Emacs, NetBeans, Qt Creator, Sublime Text, VIM, Visual Studio, and VSCode
- [Project Examples](https://docs.platformio.org/en/latest/platforms/espressif8266.html?utm_source=arduino-esp8266#examples)

### Building with make

[makeEspArduino](https://github.com/plerup/makeEspArduino) is a generic makefile for any ESP8266 Arduino project.
Using make instead of the Arduino IDE makes it easier to do automated and production builds.

### Documentation

Documentation for latest development version: https://arduino-esp8266.readthedocs.io/en/latest/

### Issues and support ###

If you encounter an issue which you think is a bug in the ESP8266 Arduino Core or the associated libraries, or if you want to propose an enhancement, you are welcome to submit it here on Github: https://github.com/esp8266/Arduino/issues.

Please provide as much context as possible, as well as the information requested in the issue template:

- ESP8266 Arduino core version which you are using (you can check it in Boards Manager)
- your sketch code; please wrap it into a code block, 
- when encountering an issue that happens at run time, attach the serial output. Wrap it into a code block, just like the code.
- for issues that happen at compile time, enable verbose compiler output in the IDE preferences, and attach that output (also inside a code block)
- ESP8266 development board model
- IDE settings (board choice, flash size)
- etc




