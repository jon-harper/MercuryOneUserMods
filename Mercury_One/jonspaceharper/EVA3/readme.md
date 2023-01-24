# EVA 3 for Mercury One

## Overview

This mod adapts EVA 3 to mount on Mercury One and adds support for stepper-mounted PCBs.

## Compatibility
### Linear Rail

MGN12C support is dropped for MGN12H, the carriage type used for Mercury One.

### Hotends

All non-Volcano hotends are compatible. Volcano support is only missing a working duct (the source STEP file has geometry flaws)

### Drive/Extruder

All drive modules are compatible.

### ABL

ABL support is currently limited to BLTouch. Initial work on a Klicky mod for the horn duct is available in `/CAD`.

### Part Fans

Support for part fans includes a 5015 fan in stock or sideways orientation.

### Shrouds and Cooling Fans

All shrouds are compatible. Both 4010 and 4020 fans may be used.

## New Parts

### Z Limit Switch Mount

This allows the bed to reach the hotend and adds additional Z height.

### X Axis Stop Block

This is a bumper for the X axis limit switch, compatible with Mercury One.

### Repository Layout

| File/Folder   | Description |
|---------------|-------------|
| readme.md     | This file   |
| changelog.md  | List of all changes |
| /CAD          | STEP files for all assemblies |
| /STL          | Printable files |
| /img          | Reference images for each assembly |

## Required Components

### Universal Front

| Part | Qty | Note |
|------|-----|------|
| front_universal_fi.stl    | 1 | |
| belt_grabber.stl          | 2 | |
| Heat Set Insert, M3x5x4   | 12 | M1/Voron-style inserts |
| Screw, M3-0.5 x 6mm SHCS  | 4  | May substitute 8mm |
| Screw, M3-0.5 x 8mm SHCS  | 2  | Only if using an ADXL |

If using a FYSETC portable input shaper, print `front_universal_pis_fi.stl` instead. This requires two (2) additional heat set inserts.

### Top for MGN12H with Endstop

This part also serves to mount the Cable Guide. An alternative version is available for those using stepper-mounted PCBs that does not have a cable guide attachment.

Note: The four (4) inserts for the Drive Mount are pressed in from the *bottom*, not the top. The added distance requires that drives mount to the top piece with 12mm screws instead of 8mm.

| Part | Qty | Note |
|------|-----|------|
| top_endstop_mgn12h.stl    | 1 | |
| cable_guide.stl           | 1 | |
| Heat Set Insert, M3x5x4   | 6 | M1/Voron-style inserts |
| Screw, M3-0.5 x 8mm SHCS  | 8 | |
| Horizontal Endstop Switch | 1 | The same as EVA 3 uses |

If using a CANBUS or other stepper-mounted PCB, print `top_endstop_mgn12h_pcb.stl` instead. This file uses two (2) fewer inserts and does not have a cable guide mount.

### Bottom Horns

Note: The Volcano horns have been modified but contain geometry errors that are beyond my ability to fix. The Source file is in the `/CAD` folder.

| Part | Qty | Note |
|------|-----|------|
| bottom_horns_fi.stl       | 1 | |
| Heat Set Insert, M3x5x4   | 1 | M1/Voron-style insert |

### Part Cooling Inlet

There are two version of this file. One is based on the stock cooling inlet; the other is mounted sideways (may save Y axis space on some configurations).

Print one (1) of:

- 5015_inlet_fi.stl
- 5015_sideways_inlet_fit.stl

Both inlets require the same materials:

| Part | Qty | Note |
|------|-----|------|
| Fan, Radial, 50mm x 15mm  | 1 | |
| Heat Set Insert, M3x5x4   | 1 | M1/Voron-style insert |
| Screw, M3-0.5 x 45mm SHCS | 4 | |
| Screw, M3-0.5 x 6mm SHCS  | 1 | May substitute 8mm. |
| Screw, M3-0.5 x 25mm SHCS | 1 | |

### Back Plate

**Note**: this piece is eliminated. The fan intake and top plate are modified in its place.

### Other Required Parts

There are no modified Drive Mounts; the standard ones will fit using 12mm screws to attach to the top piece (the front still uses 8mm).

Any hotend mount will fit the modified universal front. There is one mount modified to accept Mercury One inserts instead of EVA-style (see below).

Lastly, you will need the following for hotend cooling:

| Part | Qty | Note |
|------|-----|------|
| Fan, Axial, 40x40x10mm | 1 | Or 20mm, if preferred. |
| Screw, M3-0.5 x 12mm | 4 | If the fan is not counterbored, use 16mm. If using a 20mm fan, use 25mm. |

## Optional Components

### '36 and '42 PCB Mounts

Users of CANBUS and other stepper-mounted PCBs can use a mount with an integrated cable guide and optional shroud. Initially only NEMA17 extruders are supported.

Print one (1) of either:

- `pcb36_mount.stl`
- `pcb42_mount.stl`

For the shroud, print one (1) of either:

- `pcb_shroud.stl`
- `pcb_shroud_cat.stl`

| Part | Qty | Note |
|------|-----|------|
| `cable_guide.stl`         | 1 | |
| Screw, M3-0.5 x 8mm       | 2 | For cable guide |
| Screw, M3-0.5 x 25mm      | 2 | For stepper mount |
| Screw, M3-0.5 x 30mm      | 2 | For shroud |
| Heat Set Insert, M3x5x4   | 6 | M1/Voron-style insert |

### BLTouch Mount

Currently, only BLTouch is supported as an ABL. The universal front ABL mounting holes were moved to make room for the belts.

Nozzle offset is 12mm on the X axis and 33.5 on the Y.

| Part | Qty | Note |
|------|-----|------|
| bl_touch_mount.stl    | 1 | The file has a simple, breakways support. |
| BLTouch v3.x          | 1 | |
| Hex Nut, M3           | 2 | |
| Screw, M3-0.5 x 6mm   | 2 | May substitute 8mm. |
| Screw, M3-0.5 x 8mm   | 2 | |

### Hotend Mount: Dragon BMO / Red Lizard BMO

This is a modification of [this mod](https://www.printables.com/model/200853-eva3-dragon-hotend-mount-insert) to use M3x5x4 inserts.

| Part | Qty | Note |
|------|-----|------|
| hotend_bmo_fi.stl         | 1 | |
| Dragon BMO hotend         | 1 | |
| Screw, M2.5 x 8mm SHCS    | 4 | Usually comes with the hotend. |
| Screw, M3-0.5 x 8mm SHCS  | 4 | |
| Heat Set Insert, M3x5x4   | 4 | M1/Voron-style insert |

### Z Limit Switch Mod

This fixes the height of the limit switch so that the bumper screw works. This is only applicable for Ender 5 Pros. It has not been tested on an Ender 5 Plus.

| Part | Qty | Note |
|------|-----|------|
| z_limit_switch_cover.stl  | 1 | |
| z_limit_switch_mount.stl  | 1 | |
| Screw, M3-0.5 x 16mm SHCS | 2 | |
| Screw, M5-0.8 x 8mm SHCS  | 1 | |
| Tee Nut, Drop In, M5      | 1 | |
| Heat Set Insert, M3x5x4   | 2 | M1/Voron-style insert |
