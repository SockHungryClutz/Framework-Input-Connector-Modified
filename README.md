# Framework input shim


**This repository is a fork of [CRImier/MyKiCad/.../framework_input_brkt_smol/](https://github.com/CRImier/MyKiCad/tree/master/Laptop%20mods/framework_input_brkt_smol)**  
(It was created as a new repo so as not to copy all other KiCad projects from CRImier in the same repo)

This is a small shim for the Framework laptop motherboard. It exposes the power button,
a USB port with 5V power, keyboard backlight, Caps Lock and fingerprint LED connections.
It is designed to fit inside the outline of the input connector FPC plug,
within the motherboard outline, so that it can easily be added to existing designs.

For wire connections, this shim uses THT holes, since it's relatively easy to rip
an SMD pad off the board by pulling on a wire. With the holes positioned out from behind the
mezzanine connector, this does not require any kapton tape fix or special assembly.

Markings on the PCB: "FrmW input brkt" (shortened because the board has to be very small)

Connector used: Amphenol 10156001-051100LF

These are KiCad 9 files as these were edited with the latest version

# Changes in v3.1:

- Updated to KiCad 9
- Moved THT holes out from behind connector to eliminate all chances of THT-to-connector shorts
- Increased board height to ~10mm to make room for THT (and some PCB services require at least 1cm board size in each dimension for assembly)
- Adjust silkscreens a bit, hopefully the meaning of labels is still clear

# Changes in v3:

- Updated to KiCad 6
- Updated soldermask on connector soldering layer to decrease chances of THT-to-connector shorts
- Cosmetic: removed between-pin traces on a GND group of pins
- Adjusted traces so that there's less visual "shorts"

# Changes in v2: 

The input connector symbol numbering was incorrect
and v1 of this adapter could break your mobo or something.

- Signal names are silkscreened on the board's top layers.

- Software: Kicad 6
- Version: 2
- PCB size: 18x7.75
- Layer count: 2
