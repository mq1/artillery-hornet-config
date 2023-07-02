# artillery-hornet-config

Config changes for Marlin 2.1.2.1

To apply to https://github.com/MarlinFirmware/Configurations/tree/release-2.1.2.1/config/examples/Artillery/Hornet

Read [this](./how-to-flash.md) if you are unsure on how to flash a marlin firmware.bin

```
// Configuration_adv.h

// for octoprint
#define HOST_ACTION_COMMANDS

// enable long filenames
#define LONG_FILENAME_HOST_SUPPORT
#define LONG_FILENAME_WRITE_SUPPORT
#define SCROLL_LONG_FILENAMES

// accurate progress reporting (supports remaining times needs to be enabled in prusa slicer)
#define SET_PROGRESS_MANUALLY
#define M73_REPORT
#define SHOW_REMAINING_TIME

// for marlinbft
#define BINARY_FILE_TRANSFER
#define SDCARD_CONNECTION ONBOARD

// firmware retraction (enable use firmware retraction in prusa slicer)
#define FWRETRACT
```
