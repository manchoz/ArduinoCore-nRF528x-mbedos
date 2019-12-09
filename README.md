# Arduino Core for mbed enabled devices

The repository contains the Arduino APIs and IDE integration files targeting a generic mbed-enabled board

## Installation

Clone the repository in `$sketchbook/hardware/arduino-challenge`. The sketchbook directory is different depending on your OS:

* GNU/Linux: `$HOME/Arduino`
* MacOS: `$HOME/Documents/Arduino`
* Windows: `%USERPROFILE%\Documents\Arduino`

```bash
mkdir -p $sketchbook/hardware/arduino-challenge
cd $sketchbook/hardware/arduino-challenge
git clone git@github.com:manchoz/ArduinoCore-mbed -b challenge mbed
```

Then clone https://github.com/arduino/ArduinoCore-API in a directory at your choice. Checkout `namespace_arduino` branch.

```bash
git clone git@github.com:arduino/ArduinoCore-API -b namespace_arduino
```

Remove the symlink to `api` you can find in  `$sketchbook/hardware/arduino-challenge/mbed/cores/arduino` and replace it with a symlink to `ArduinoCore-API/api`

Open Arduino IDE; you should now see a new "Challenge PMC R2DX" target under `Arduino Challenge Boards (Mbed OS)` label (scroll down if needed).
