# Poor mans BashBunny with RGB-LED

forked from x821938/PoorMansBashBunny

All credits belong there!

The purpose of this fork is to get a better support of the bunny script language.

## Read more about the original project here:

Read all about the project at https://www.cron.dk/poor-mans-bash-bunny/

For very little money (about 1/10th of the real BashBunny) you can make a clone with many of the same powerfull features.

## Images

![PoorMansBashBunny with RGB LED](https://raw.githubusercontent.com/schneebonus/PoorMansBashBunny/master/images/poorbunny.jpg)
Image of my poorly soldered Bunny with a Frankenstein-Resistor-Constructions (3 x 470 Ohm would be a better solution).
Buttons and dip-switches are similar to the original project but I removed the two single-color leds and replaced them with one rgb led.

![Example usage of LED](https://raw.githubusercontent.com/schneebonus/PoorMansBashBunny/master/images/bashbunny_rickroll.png)
Example usage of the LED command. It should support the bashbunny colors and modes.

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

## Install
```
> sudo su
# apt install -y git
# git clone https://github.com/x821938/PoorMansBashBunny.git /bunny
# cd /bunny
# ./setup.sh
```

## Cool ideas for the future:
- User zero pi w to open a wifi hotspot and allow some kind of remote control
- Add an i2c display
