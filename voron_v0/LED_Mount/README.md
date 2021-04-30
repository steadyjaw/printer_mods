# v0 - LED strip mount

this mod was tested on a v0.0 ... but it is should fit to a v0.1 as well.
It is mounted to the top/side extrusions and brings ligth to the inside of the printer.
If you use neopixel each LED will be addressable indivudually. You will find some simple klipper macro inspiration in  `./firmware/`

This mount consists out off 2 mounts. Left and Right.
each one:
- easily fits 7 LEDs of RGB(W) LED Strip 60 led/m 
- uses 2 mm acrylic sheet (118mm * 12mm) ... you can scuff it. The light will get diffused a little bit

## Instructions
1. print parts
Print parts upside down. Should be printable without supports. Pay attention to bridges...
![SLICER1](/voron_v0/LED_Mount/images/slicer1.png?raw=true) ![SLICER2](/voron_v0/LED_Mount/images/slicer2.png?raw=true)
2. create acrylic sheets
They propably won't fit, even if the dimensions are spot on. Grind them down on some sandpaper until they fit into the slot.
3. solder LED strips
They can be daisy-chained ... by doing that, you only need to use one GIO on you board and even can get an data-out to even get more LEDs chained to it. That's how I wired my LED strip:
![WIRE](/voron_v0/LED_Mount/images/wired.png?raw=true)
4. assemble everything
5. mount it with 6 additional M3x6mm screws
You need to add M3 nuts to the top extrusions

## Images
![IMAGE](/voron_v0/LED_Mount/images/image1.jpg?raw=true)
![IMAGE](/voron_v0/LED_Mount/images/image2.jpg?raw=true)
![IMAGE](/voron_v0/LED_Mount/images/image3.jpg?raw=true)
![IMAGE](/voron_v0/LED_Mount/images/image4.jpg?raw=true)