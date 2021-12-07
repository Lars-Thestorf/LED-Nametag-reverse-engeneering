# LED-Nametag-reverse-engeneering
Reverse Engeneering a sertronics led-nametag

By the time of writing this its 07.12.2021

Back in 2018 I bought an LED Nametag on Maker Faire Hannover.

More or less immideately i started reverse Engeneering the USB protocol since I wanted to be able to configure it on the go.

I wrote a simple Android application which was able to do so. Link...

A few Days ago i decided to take a look at it again because my device has some issue with discharging when not in use.

# Physical
11x44 LEDs

Power-Button

Mode-Button

Micro USB port

# Behaivior
short press power = on/off (does not work if charging)

long press power = same as short press

short press mode = cycle modes

long press mode = cycle brightness

# Technical
MM32L050FP ARM Microcontroller

11x44 charie-plexed LED-Matrix connected directly to the Microcontroller, no form of driver IC or even current limiting resistor present.

USB 2.0 full speed device vid:0x0416, pid:0x5020, Manufacturer: "LSicroelectronics", Product: "LS32 Custm HID"

Descriptor...

Protocoll...

# Bootloader
pressing Mode-Button while nametag is turned off and connecting usb makes chip enter some kind of bootloader mode.

Mode-Switch can be released afterwards.

USB 2.0 full speed device vid:0x0483, pid:0x5740, Manufacturer: "MindMotion", Product: " MM32 Virtual COM Port"

exit bootloader via pressing Mode button again (nametag will be on afterwards) or disconecting usb (nametag will be off afterwards).

# Hardware
250mAh Lipo Battery

DW06K Lipo Protection IC



Schematic...
