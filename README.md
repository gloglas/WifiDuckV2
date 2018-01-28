# [ WIP ] WifiDuckV2
Rewrite of spacehuhn's project.

I added some features I missed.

## What is better?
Mouse control

You can write ASCII code in your scripts!

OS detection and more!

# Instalation
First see this project! https://github.com/spacehuhn/wifi_ducky#installation

You will need this library: https://github.com/keyboardio/FingerprintUSBHost

# Syntax

## OS Detection
OS - Dump fingerprint (Better to write it as first line)

WINDOWS - Start code below if it is Windows machine.

MACOS - Start code below if it is iOS machine.

LINUX - Start code below if it is Linux machine.

OSEND - End the os code

### Example
```Duckyscript
OS
STRING I do not care now.

WINDOWS
STRING I am Windows machine.
OSEND

LINUX
STRING I am Linux/Android/ChromeOS machine.
OSEND

STRING I do it anyway.

MACOS
STRING I am iOS machine.
OSEND
```

## ASCII
ASCII - write ASCII code
```Duckyscript
REM write 'a'
ASCII 97
```
## Digital & Analog write
DPIN - Same as digitalWrite(pin,value); in Arduino IDE.

APIN - Same as analogWrite(pin,value); in Arduino IDE.

MPIN - Same as pinMode(pin,mode); in Arduino IDE.

```Duckyscript
MPIN 2 OUTPUT
MPIN 2 INPUT
DPIN 2 HIGH
APIN A0 200
```

## MOUSE
MOUSE X Y - Move mouse in both directions.

MOUSEX X - Move mouse only in X-axis.

MOUSEY Y - Move mouse only in Y-axis.

SCROLL Y - Scroll.

CLICK - Press MOUSE1.

CLICK_RIGHT - Press MOUSE2.

CLICK_MIDDLE - Press MOUSE3.

MOUSE_CLICK_LEFT, CLICK_LEFT - aliases for all 3 buttons.

PRESS - Hold MOUSE1.

MOUSE_PRESS_LEFT, PRESS_LEFT - aliases for all 3 buttons.

RELEASE - Release MOUSE1

MOUSE_RELEASE_LEFT, RELEASE_LEFT - aliases for all 3 buttons.

```Duckyscript
MOUSE 2000 -400
CLICK
SCROLL 20
PRESS
MOVE -100 2500
RELEASE_LEFT
CLICK_RIGHT
```
## NUMPAD
NUM_0-9 - Press numpad numbers.

ASTERIX, MINUS, SLASH - Press symbols

```Duckyscript
SLASH
SLASH
SPACE
NUM_2
NUM_0
NUM_1
NUM_8
```

## Numbers for Czech layout.
CZ_0-9 - Press numbers.

## License
This project is licensed under the MIT License - see the [license file](LICENSE) file for details

## Sources and additional Links

The USB Rubber Ducky: https://hakshop.com/products/usb-rubber-ducky-deluxe

Seytonic: http://youtube.com/seytonic
          https://github.com/seytonic
          
Spacehuhn: https://github.com/spacehuhn/
           https://github.com/spacehuhn/wifi_ducky
          
Arduino Ducky Script interpreter: https://github.com/Seytonic/Duckduino-microSD

Jesse Vincent (os detection): https://github.com/keyboardio/FingerprintUSBHost

Cnlohrs ESP8266 USB Software Driver: https://github.com/cnlohr/espusb
