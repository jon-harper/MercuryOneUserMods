# EVA 3 for Mercury One

## Overview

This mod adapts EVA 3 to mount on Mercury One. It is still in testing.

### Repository Layout

| File/Folder   | Description |
|---------------|-------------|
| readme.md     | This file   |
| changelog.md  | List of all changes |
| /CAD          | STEP files for all assemblies |
| /STL          | Printable files |
| /img          | Reference images for each assembly |

## Components

### Required

#### Universal Front

| Part | Qty | Note |
|------|-----|------|
| front_universal_fi.stl    | 1 | |
| belt_grabber.stl          | 2 | |
| Heat Set Insert, M3x5x4   | 12 | M1/Voron-style inserts |
| Screw, M3-0.5 x 8mm SHCS  | 4  | Add two (2) more if using an ADXL |

#### Top for MGN12H with Endstop

This part also serves to mount the Cable Guide.

Note: The four (4) inserts for the Drive Mount are pressed in from the *bottom*, not the top.

| Part | Qty | Note |
|------|-----|------|
| top_endstop_mgn12h.stl    | 1 | |
| cable_guide.stl           | 1 | |
| Heat Set Insert, M3x5x4   | 6 | M1/Voron-style inserts |
| Screw, M3-0.5 x 8mm SHCS  | 8 | |
| Horizontal Endstop Switch | 1 | The same as EVA 3 uses |

#### Bottom Horns

The Volcano horns have not yet been modified.

| Part | Qty | Note |
|------|-----|------|
| bottom_horns_fi.stl       | 1 | |
| Heat Set Insert, M3x5x4   | 1 | M1/Voron-style insert |

#### Part Cooling Inlet

There are two version of this file. One is based on the stock cooling inlet; the other is mounted sideways (may save Y axis space on some configurations).

Print one (1) of:

- 5015_inlet_fi.stl
- 5015_sideways_inlet_fit.stl

Both inlets require the same materials:

| Part | Qty | Note |
|------|-----|------|
| Fan, Radial, 50mm x 15mm  | 1 | |
| Heat Set Insert, M3x5x4   | 1 | M1/Voron-style insert |
| Screw, M3-0.5 x 40mm SHCS | 4 | |
| Screw, M3-0.5 x 6mm SHCS  | 1 | |
| Screw, M3-0.5 x 25mm SHCS | 1 | |

#### Back Plate

**Note**: this piece is eliminated. The fan intake and top plate are modified in its place.

#### Other Required Parts

There are no modified Drive Mounts; the standard ones fit normally. You will still need to choose and print one.

Any hotend mount will fit the modified universal front. There is one mount modified to accept Mercury One inserts instead of EVA-style (see below).

Lastly, you will need the following for hotend cooling:

| Part | Qty | Note |
|------|-----|------|
| Fan, Axial, 40x40x10mm | 1 | Or 20mm, if preferred. |
| Screw, M3-0.5 x 12mm | 4 | If the fan is not counterbored, use 16mm. If using a 20mm fan, use 25mm. |

### Optional

#### BLTouch Mount

Currently, only BLTouch is supported as an ABL. The universal front ABL mounting holes were moved to make room for the belts.

| Part | Qty | Note |
|------|-----|------|
| bl_touch_mount.stl    | 1 | The file has a simple, breakways support. |
| BLTouch v3.x          | 1 | |
| Hex Nut, M3           | 2 | |
| Screw, M3-0.5 x 6mm   | 2 | May substitute 8mm. |
| Screw, M3-0.5 x 8mm   | 2 | |

#### Hotend Mount: Dragon BMO / Red Lizard BMO

This is a modification of [this mod](https://www.printables.com/model/200853-eva3-dragon-hotend-mount-insert) to use M3x5x4 inserts.

| Part | Qty | Note |
|------|-----|------|
| hotend_bmo_fi.stl         | 1 | |
| Dragon BMO hotend         | 1 | |
| Screw, M2.5 x 8mm SHCS    | 4 | Usually comes with the hotend. |
| Screw, M3-0.5 x 8mm SHCS  | 4 | |
| Heat Set Insert, M3x5x4   | 4 | M1/Voron-style insert |