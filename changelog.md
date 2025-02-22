**2025.02.21 (1.37)**
- Correct block size calculation for block selection to prevent selection larger than 1/2 screen in either direction
- Added block copy, and block paste
- Rewrote block inverse to improve performance, and reduce code size.
- Added ability to change background and text color
- Added non-ctrl up/down/left/right to block selection for easier selection.
- Changed editor nav from ctrl+up/down/left/right to up/down/left/right (minus/equal/plus/asterisk)
- Remapped option and status dialogs - now OPTION and SELECT respectively
- Reorganization of user manual, improvements to text, and improvements to table of contents.

**2025.02.17 (1.30)**
- Added support back in for verified terminal displayable specials: ESC, Up, Down, Left, Right, Inv Up, Inv Down, Inv Left, Inv Right, Inv Tab, Inv Del
- Added block selection toggle
- Added block status to status dialog
- Added block operations: clear, inverse, fill, mirror, flip (upside down)

**2025.02.16 (1.20)**

- Fix bad mapping of Control-w.  Remapped wipe keystrokes.  Now using Shift-Control-W, F, R.
- Disallow unused Control-2 through 9 and 0.
- Removed handling of special screen control characters.  Not displayable unless escaped.
- Added Get Char at cursor, and Put Char at cursor for single character copy/paste. (Shift-Control-G/P)
- Added Inverse toggle of character at cursor.
- Rewrote Load and Save routines.
- Fixed hang after load if end line marker is set when load begins.
- Fixed load not resetting end line marker to off when load complete.
- Fixed user manual references of ENTER to RETURN.

**2025.02.12 (1.11)**

- Fix missing terminator in file load name input variable.
- Fixed broken load from 1.10 (over optimized ATASCII to internal routine).
- Fixed ESC char as 1st byte when loading file with newline as first line.
- Set X,Y references to 0 based for continuity with "zero"ing cursor position.

**2025.02.12 (1.10)**

- Added Inspect character under cursor
- Change menu and dialog verbiage from Column/Row Fill to Fill Column/Row
- Updated control key map.

**2025.02.11 (1.09)**

- Increase soft click duration to eliminate ~10% no sound rate
- Set default cursor location to middle of screen (home)
- Remapped Ctrl-H (home cursor) to Shift-Control-H
- Added Shift-Control-0 to zero cursor (position 0,0)
- Set Fills (background, row, col) to prepopulate input with value of char under cursor

**2025.02.10 (1.08)**

- Added Center row

**2025.02.09 (1.07)**

- Remap some keys to allow entry of specific high value ATASCII codes (arrows, etc).

**2025.02.09 (1.06)**

- Restrict ControlShift keys from input to prevent invalid chars from being entered

**2025.02.08 (1.05)**

- Added fill row
- Added fill column

**2025.02.08 (1.04)**

- Corrected status and prefs reflection of key click (was opposite)

**2025.02.07 (1.03)**

- Fixed restore of key click on exit (was setting 1, should have been 0)
- Added XL/XE check

**2025.02.07 (1.01)**

- Fixed issue with garbage line appearing when exiting file Load without loading.

