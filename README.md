# Poor mans BashBunny with RGB-LED

forked from x821938/PoorMansBashBunny

All credits belong there!

## Read about the original project here:

Read all about the project at https://www.cron.dk/poor-mans-bash-bunny/

For very little money (about 1/10th of the real BashBunny) you can make a clone with many of the same powerfull features.

## Changes I made:
- Changed GPIO-PINs
- RGB led instead of two single-color leds
- Support for a RGB-LED (compatible to bash bunnys LED-command)
- Added RUN command from hak5
- Increased size of STORAGE to 256MB
- Set an alias Q=QUACK (for better bunnyscript support)
- Started adding a german keyboard layout

## GPIO-Layout:
(specified in bin/bunny-launcher.py)
- LED_RED to GPIO5
- LED_GREEN to GPIO11
- LED_BLUE to GPIO9
- button_green to GPIO13 and GND
- button_red to GPIO19 and GND
- DIP-Switches to GPIO2, GPIO3, GPIO4, GPIO17 and GND

## Cool ideas for the future:
- User zero pi w to open a wifi hotspot and allow some kind of remote control
- Add an i2c display
