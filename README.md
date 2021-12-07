# LED-Nametag-reverse-engeneering
Reverse Engeneering a sertronics led-nametag

# Physical
11x44 LEDs
Power-Button
Mode-Button
Micro USB port
MM32L050-FP ARM Microcontroller

# Behaivior
short press power = on/off (does not work if charging)
long press power = same as short press
short press mode = cycle modes
long press mode = cycle brightness

# Technical
USB 2.0 full speed device vid:0x0416, pid:0x5020, Manufacturer: LSicroelectronics, Product: LS32 Custm HID
Descriptor...
Protocoll...

# Bootloader
pressing Mode-Button while nametag is turned off and connecting usb makes chip enter some kind of bootloader mode
Mode-Switch can be released afterwards
USB 2.0 full speed device vid:0x0483, pid:0x5740, Manufacturer: MindMotion, Product:  MM32 Virtual COM Port
exit bootloader via pressing Mode button again (nametag will be on afterwards) or disconecting usb (nametag will be off afterwards)

# Hardware
Schematic...
