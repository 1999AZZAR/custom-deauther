# Custom Deauther

Custom Deauther is a project that allows you to create your own deauthentication device using an ESP8266 board and a 3D-printed case. A deauthentication device can be used to disconnect devices from a WiFi network by sending deauthentication packets.

## Features

- Scan for nearby WiFi networks and devices
- Select a target network or device to deauthenticate
- Monitor the status of the deauthentication attack
- Customize the settings of the device, such as LED brightness, channel hopping, and packet rate
- Use a web interface or an OLED display to control the device

## Requirements

To build your own custom deauther, you will need:

- An ESP8266 board (such as NodeMCU or Wemos D1 Mini)
- A 3D printer and filament
- A micro USB cable
- A soldering iron and some wires
- A computer with Arduino IDE installed

## Installation

1. Download or clone this repository to your computer.
2. Open the `custom-deauther.ino` file with Arduino IDE.
3. Install the required libraries from the `libraries` folder using Sketch > Include Library > Add .ZIP Library.
4. Select your ESP8266 board and port from Tools menu.
5. Upload the sketch to your board.
6. Connect an OLED display to your board (optional) by following this wiring diagram: https://github.com/1999AZZAR/custom-deauther/blob/master/wiring.png
7. Print the case parts from the `case` folder using your 3D printer.
8. Assemble the case and insert your board into it.

## Usage

To use your custom deauther, follow these steps:

1. Turn on your device by plugging it into a power source or a battery pack.
2. Connect to its WiFi network using any device with a browser (the default SSID is `pwned` and password is `deauther`).
3. Open http://192.168.4.1 in your browser to access the web interface.
4. Scan for nearby WiFi networks and devices by clicking on Scan button.
5. Select a target network or device by clicking on its name in the list.
6. Start a deauthentication attack by clicking on Attack button.
7. Stop the attack by clicking on Stop button.

Alternatively, you can use the OLED display and buttons to control your device:

1. Press any button to wake up the display.
2. Use left and right buttons to navigate through different menus (Scan, Attack, Settings).
3. Use up and down buttons to scroll through items in each menu.
4. Press middle button to select an item or confirm an action.

## Disclaimer

This project is for educational purposes only. Do not use it for illegal or malicious activities. I am not responsible for any damages or consequences caused by using this device.

<!--
## License

This project is licensed under GNU General Public License v3 - see [LICENSE](https://github.com/1999AZZAR/custom-deauther/blob/master/LICENSE) file for details.
-->

## Acknowledgments

This project is based on [Spacehuhn's ESP8266 Deauther](https://github.com/SpacehuhnTech/esp8266_deauther), which is an awesome project that inspired me to create my own version with some modifications and improvements.
