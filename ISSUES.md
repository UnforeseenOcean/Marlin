# Issues with this fork of Marlin 1.1.8

This document will show what went wrong with this specific fork of Marlin firmware.

## Issues found

- ~~Auto home command is delayed and only X axis tries to home~~
  - ~~Driver connection issue, not sure about Z axis though.~~
   - Yup, definitely a driver connection issue. Not so sure about why it's doing that.
   - Note about extruder motor not turning while hotend is cold: It's supposedly normal. Just heat the nozzle up to the temperature and try again.
- ~~Auto home does not move the X and Y axis to correct position~~
  - SOLVED: `#define Z_SAFE_HOMING` is used for center positioning while auto homing on Marlin 1.1.8.
