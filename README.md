# WifiDuckV2
Rewrite of spacehuhn's project.

First see and support this guy! https://github.com/spacehuhn/wifi_ducky

## What is better?
Mouse control
You can write ASCII code in your scripts!
OS detection!!

# Syntax
## ASCII
ASCII - write ASCII code
```Duckyscript
REM write 'a'
ASCII 97
```
## OS Detection
OS - to dump os fingerprint (Better to write it as first line)

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
