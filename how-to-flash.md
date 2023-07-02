# WIP

How I flashed firmware.bin to my Artillery Hornet

## Requirements

- A device with Octopi (I'm using a Raspberry Pi 3B+) connected to the printer via usb

## Steps

- from the Octoprint terminal send the M997 command to put the printer in dfu mode
- scp the firmware.bin to the device running octopi
- ssh into the device and install the dfu-util package using apt
- with `dfu-util --list` make sure the flash device is at index 0 (otherwise edit the next command)
- run dfu-util -a 0 -D firmware.bin -s 0x08000000

## Credits

- https://www.reddit.com/r/Artillery3D/comments/onicqu/comment/ig56rm6/?utm_source=share&utm_medium=web2x&context=3
- https://techoverflow.net/2021/10/09/how-to-flash-stm32-platformio-firmware-using-dfu-util/
