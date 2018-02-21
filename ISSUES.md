# Issues with this fork of Marlin 1.1.8

This document will show what went wrong with this specific fork of Marlin firmware.

## Issues found

- ~~Auto home command is delayed and only X axis tries to home~~
  - ~~Driver connection issue, not sure about Z axis though.~~
   - Yup, definitely a driver connection issue. Not so sure about why it's doing that.
- ~~Auto home does not move the X and Y axis to correct position~~
  - SOLVED: `#define Z_SAFE_HOMING` is used for center positioning while auto homing on Marlin 1.1.8.
