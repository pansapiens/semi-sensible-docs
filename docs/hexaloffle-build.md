# Hexaloffle DIY build guide

_TODO: This section will contain DIY build instructions and a link to the iBOM_

## Hardware development


## Exporting from KiCad for production

- Run DRC - correct any issues. Some silkscreens are expected to overlap (jacks) and there will be unconnected nets between boards (eg `OUTJACK_1` etc) - but be careful ignoring anything.
  - ***TODO:*** Edit jack silkscreens to remove overlapping parts when sharing GND, avoid that warning.

- Boards are all in a single PCBnew file since this has advantages at design time. To export a single board, simply delete the others (but don't save !) then export gerbers etc.

- Gerbers, BOMs and position files for production were exported using [kicad-jlcpcb-tools](https://github.com/Bouni/kicad-jlcpcb-tools) 
  - Alternative to consider for the future: [JLC-Plugin-for-KiCad (Fabrication Toolkit)](https://github.com/bennymeg/JLC-Plugin-for-KiCad) - since part offsets and rotations can defined in the symbol fields and footprint properties for better reproducibility of exports.

## Trivia

*NOTE*: Early prototypes of the Hexaloffle were internally named 'Picorack Modulator' - you may see reference to this in some of the design and source files.

