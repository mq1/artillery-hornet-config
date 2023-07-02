# artillery-hornet-config

Config changes for Marlin 2.1.2.1

To apply to https://github.com/MarlinFirmware/Configurations/tree/release-2.1.2.1/config/examples/Artillery/Hornet

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

// for marlinbft
#define BINARY_FILE_TRANSFER
#define SDCARD_CONNECTION ONBOARD
```
