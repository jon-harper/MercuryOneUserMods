# EVA 3 for Mercury One.1

## Changelog

## 23/01/13

- Fit test appears ready for testing on a working Merc.
- Added cutout in belt grabber for divider between belts.
- Added a version of the cable guide post with the guide to the side.

## 23/01/12

- Tweaked post again for cable guide.
- Spent most of the day fixing a printer.

### 23/01/11

- Tagged all parts in the Fusion model with part numbers to scrape BOM data.
- Tweaked BLTouch mount to add a little more material.
- Added a readme with BOM info.
- Added a chamfer to the top piece insert holes and an overhang for the endstop mount.
- Test fitting went well:
    - Found & fixed missing BLTouch holes in the front piece.
    - Made cable guide tower thinner to avoid blocking drive piece.
    - Rotated cable guide around to face completely backwards.
- Added CAD files for Volcano duct.
    - The duct source file has broken geometry that I am unable to fix.
    - I have made the changes otherwise needed to make the duct compatible.

### 23/01/10

- Started changelog
- Switched M3 inserts to Mercury One-style to simplify BOM.
    - All parts now use M3x5x4mm inserts.
    - Added Dragon BMO part with resized insert holes.
- Refactored Fusion 360 files;
    - Split out small Core parts into individual files
    - Removed a lot of quick hacks
- Added divider to belt grabber between belts.
- Re-oriented parts to export in the correct orientation for print.
- Endstop is now EVA-style horizontal and mounted on the right.
    - Ditched rear-mounted endstop design.
    - Still need to design a bumper for the endstop.
- Cable guide improvements:
    - Rotated guide mount 45 degrees to stay out of the way of endstop.
    - Closer to rear toolhead and takes less X axis space.
    - Raised cable guide 15mm.
    - Rear of cable guide allows for larger zip ties.
- BLTouch mount:
    - Moved mount points over belt clamp
    - Design a new BLTouch mount
    - Uses a simple cutaway support structure

### 23/01/07

- Started work
