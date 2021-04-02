# Voron V0 - Skirt Mod with 0.96" OLED
Yet another Display Mod... 
There is already such a mod on the [VoronDesign Users Repo](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/),  but this one is printable on the V0 ;)

## Pictures
![Exploded](/0.96_OLED_Skirt_Mod/images/cad_view.png?raw=true)

![Real](/0.96_OLED_Skirt_Mod/images/live_view.png?raw=true)

## STLs
In order to print this MOD you only need to print this 3 Parts:
- Diplay Mount
- 2 shortend Skirts
```
./STL/[a]_Display_mount_x1.stl
./STL/skirt_frontleft_x1.stl
./STL/skirt_frontright_x1.stl
```

The other STLs in this Repo are normal skirt files, with holes in the bottom.
They're way easier to mount, this way. :)

```
./STL/skirt_side_mirror_w_holes_x2.stl
./STL/skirt_side_w_holes_x2.stl
```


## Printer Config (SKR E3 mini v2.0)

```
[display]
lcd_type: ssd1306
i2c_mcu: mcu
i2c_bus: i2c1a
```
