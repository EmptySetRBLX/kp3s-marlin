# Marlin firmware for Kingroon KP3S 3.0

Modified version of https://github.com/konradmb/kp3s-marlin

---
Built from source using lts-2.1.2

Builds using maple to avoid DMA sd card read issue

Will need to rotate the screen, or just use the screen from the side.

## Download
Download `robin_nano.bin` file from [Releases](https://github.com/EmptySetRBLX/kp3s-marlin/releases).

### Installing
Put `robin_nano.bin` file to the root of SD card, turn on printer and wait for flashing to complete.
You can always go back to the stock firmware by dowloading it from Kingroon website.

## Features
- Manual mesh bed leveling with 7x7 grid. Why buy 3D Touch when you can do the same by yourself?
- Linear Advance
- Pre-calibrated E-steps. I've set it to 833.7 steps/mm (factory is 768). Change it in menu if it doesn't work for you.
- Pre-calibrated XY bed skew compensation. Change it in menu if it doesn't work for you.
- MPC hotend temperature control (bed is still PID). Zero overshoot, maintains precise set-point compared. You can run auto-tune in menu if it doesn't work correctly.
- Nozzle park, pause and filament change.
- Bezier curve and arc GCode support.
- Print most-recent file pop-up on SD card plug.
- Plug heatsink fan to PB0 pin and get fan auto-shutdown when hotend is cool.
- And more… (checkout config files in [/config](https://github.com/EmptySetRBLX/kp3s-marlin/tree/master/config) directory) 
