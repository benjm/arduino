# Programming an Arduino-lite Adafruit Trinket
Following guides from [Adafruit](https://learn.adafruit.com/introducing-trinket/introduction) and [Arduino.cc](https://www.arduino.cc/en/Guide/Windows)

## Getting going
Arduino IDE from [Arduino.cc](https://www.arduino.cc/en/Main/Software)

Adafruit driver (necessary on Windows only from https://learn.adafruit.com/adafruit-arduino-ide-setup/windows-setup) installed both as not clear which one of the "Gemma" drivers is the trinket one. Trinket has a Teal board but the "black board gemma" section is the only bit ot mention the trinket. Anyway...

wasn't working, moved the usb cable to a different usb port after installing the two drivers, detected correctly as USBTiny

In the arduino IDE, preferences, add the [Adafruit trinket board info](https://adafruit.github.io/arduino-board-index/package_adafruit_index.json)

The in the board manager, install the adafruit (may take a short while to appear, probably downloading and parsing the json)

Finally the Trinket 8MHz should be selectable

## Programming something easy
Select the correct board (Trinket 8MHz)
Select the correct Programmer (USBtinyISP)

Some sort of error, supposedly to do with the bootloader mode not being selected. Tried pressing the button to get the red light to flash (bootlader mode) but it would only flash for a short while then go off again. Windows complained about USB device errors when I did this.

After a reboot of the laptop I tried agagin. Also tried running the "burn bootloader command" in the IDE. This threw up some other error, however, this time around pressing the trinket button seemed to leave it in flashing-red-bootlader-ready mode ant the basic "blink" programme uploaded to it just fine.

## Setting up for testing using a bread board


