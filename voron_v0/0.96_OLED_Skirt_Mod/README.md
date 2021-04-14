
# Voron V0 - Skirt Mod with 0.96" OLED
Yet Another Display Mod...
There is already a skirt mod for an 0.96" OLED on the [VoronDesign Users Repo](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/), but this one is printable on the V0!

## Pictures

![CAD](/voron_v0/0.96_OLED_Skirt_Mod/images/cad_view.png?raw=true)

![REAL](/voron_v0/0.96_OLED_Skirt_Mod/images/live_view.png?raw=true)

### Optional Display Mounts
![VARS](/voron_v0/0.96_OLED_Skirt_Mod/images/vars_view.png?raw=true)


## Printing

You need to print 3 parts:
- 1x display mount (you may use accent color)
- 2x shortened skirts (lef and right)

## Assembly
 1. Mounting OLED to printed Part.
 2. Insert 2 BHCS M3 x6 to the display mount
 3. Use two `M2x10 Self Tapping Screws for Plastic` from BOM and snap like 6-7mm off of it. Fasten OLED with them.
 2. Remove old Skirt in the front
 3. Add two M3 nuts to the extrusion, where the shortened skirts and the display mount will be mounted to
 4. Bolt 3 new parts to extrusion.
You'll need two erxtra M3 screws for that!

![EXPLODED](/voron_v0/0.96_OLED_Skirt_Mod/images/exploded_view.png?raw=true)

## Connection and firmware
### SKR mini E3 v2
There are a few options to connect the display to your MCU. This is one way.
Make sure the pins are connected correctly:
|Display|MCU|
|--|--|
|GND|GND (EXP1)|
|VCC|+5V (EXP1)|
|SCL|PB8 (EXP1)|
|SDA|PB9 (EXP1)|

![CONNECTION](/voron_v0/0.96_OLED_Skirt_Mod/images/connection_skr_mini_e3_v2.png?raw=true)

#### printer.cfg for Klipper
You either copy the 2 config files located in the folder `./fimware/SKR_mini_E3_v2/` to you klipper configuration folder and add the following to you `printer.cfg`:
```
[include display.cfg]
[include display_data.cfg]
```
**Alternatively**, you just can add this to you `printer.cfg`:
```
[display]
lcd_type: ssd1306
i2c_mcu: mcu
i2c_bus: i2c1a
```