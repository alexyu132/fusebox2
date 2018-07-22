# FuseBox2
A new CoreXY 3D printer design.
![FuseBox2 Render](image/render.jpg)

## Specifications
* Rigid 2020(top and sides)/2040(bottom) aluminum extrusion frame
* Non-crossing CoreXY belt path
* 210x200x210mm build area
* 390x340x412mm size
* PCB heatbed with 3 point leveling
* Powerful 2040 part cooling blower
* E3D V6 or Lite6 + Bowden extruder
* 24v + 32 bit electronics recommended

## Additional features (FuseBox 2R upgrade)
* Lightweight and quiet MGN12 rail gantry
* >5mm more Y travel, 3mm less Z travel than stock
* Modular fan duct

## Improvements over original FuseBox
* Slightly more compact
* Slightly larger build area
* Much greater frame and z axis rigidity
* Belt tensioning improvements - much easier to tension and screw-clamped to prevent slipping out
* Clamped bearing and rod mounts - no more structural zip ties
* Proper belt idlers - eliminates belt rubbing
* Extrusions (optionally) joined via tapped ends + screws instead of corner brackets
* Lowered part count
* Vertical gantry for easier hotend installation/removal and better cooling
* Better endstop mounting

# FuseBox2R rail gantry upgrade
![FuseBox2 Render](image/2R.jpg)

Switches out the twin 8mm rods on the gantry for a single MGN12 rail. Improvements include ~30% gantry weight savings for less ringing and higher speeds, lowered bearing noise, easier belt tensioning, and a modular fan duct. Relatively inexpensive (~$10-$15) MGN12 rails can be found on Aliexpress, so it's recommended to build this configuration if starting from scratch. The printed parts for the 2R gantry are in the r-gantry subfolder in the stl folder. If building from scratch, you can move these files into the stl directory to replace the old rod gantry parts with the new rail gantry parts.

## Changes
The entire CoreXY movement will need to be changed out. This includes all the parts on the gantry itself as well as the motor mounts and idler blocks.

The 2R design now homes to the back right side, so you'll need to change the firmware to home to X max instead of min. The belts are also a bit shorter, so you may need to cut them slightly. 

# BOM

| Item | Quantity  |
|-----------------------------------------------------------------------------------------|----------|
| **Extrusions**  |
| 2020 extrusion, 350mm | 2  |
| 2020 extrusion, 340mm | 6  |
| 2020 extrusion, 184mm | 1  |
| 2020 extrusion, 202mm | 2  |
| 2040 extrusion, 184mm | 1  |
| 2040 extrusion, 350mm | 2  |
| 2040 extrusion, 300mm | 2  |
| **Heaters, motors, electronics**  |
| MK2 compatible PCB heatbed | 1  |
| 15A 24v PSU or 30A 12v PSU | 1  |
| E3DV6 compatible hotend with PTFE tube and coupler | 1  |
| Any electronics (32 bit preferred, mounts available for azsmz board+lcd) | 1  |
| NEMA 17 stepper (60+ oz in/42+ N cm preferred) | 3  |
| NEMA 17 short body stepper (up to 30mm motor body length) | 1  |
| IEC socket with fuse and switch | 1  |
| ~5A 250v fuse | 1  |
| IEC power cord | 1  |
| Mechanical endstop (Note: remove the microswitch from one of them to use on the x axis) | 3  |
| 40mm axial fan | 1  |
| 2040s radial blower | 1  |
| Thermistor for heatbed | 1  |
| **Mechanical**  |
| 8mm OD smooth rod, 300mm length | 6  |
| LM8LUU linear bearing | 6  |
| T8 leadscrew+nut, 250mm length, 2mm pitch preferred | 1  |
| 16T GT2 idler for 6mm belt(6 toothed/2 smooth or 8 smooth) | 8  |
| 20T GT2 pulley for 6mm belt | 2  |
| 3m GT2 belt, 6mm | 1  |
| 625zz bearing | 1  |
| 5mm to 8mm flex coupler | 1  |
| MK8 extruder gear | 1  |
| **Fasteners and Hardware**  |
| M5x8mm button head bolt | 51  |
| M5x12mm button head bolt | 28  |
| M5 T nuts (drop-in recommended) | 51  |
| M3x8mm socket head bolt | 16  |
| M3x10mm button head bolt | 36  |
| M3x25mm button head bolt | 13  |
| Bed leveling spring, nut, and bolt set | 3  |
| Extruder spring | 1  |
| M3 locknut | 48  |
| Adhesive felt feet | 4  |
| **Misc**  |
| ~200x213mm glass sheet | 1  |
| ~200x213mm PEI sheet with adhesive | 1  |
| Zip ties | Varies  |
| Cable mesh (optional) | Varies  |
| 18AWG wire for AC input | Varies  |
| 14AWG wire for heatbed and main DC power | Varies  |
| Small binder/bulldog clips | 4  |

# FuseBox2R MGN12 upgrade BOM

| Item                            | Quantity |
|---------------------------------|----------|
| 250mm MGN12 Rail + MGN12C Block | 1        |
| M3x10mm bolt                    | 2        |
| M3x6mm bolt (socket head)       | 4        |
| M3 lock nut                     | -2       |
| M3x25mm bolt                    | -4       |
| 300mm 8mm smooth rod            | -2       |
| LM8LUU bearing                  | -2       |

Note that the upgrade requires new fasteners and parts, but also gets rid of some. If upgrading, get only the positive quantity items. If building from scratch, add item amounts to base BOM.
