# Bootloader Manual Guide for Users

## How to Use the Bootloader
This guide follows the DFU button check behavior used by `dfu_button_check`.
The bootloader checks the button at startup and then chooses one of three behaviors:
- boot directly to the application
- enter DFU update mode
- perform a self-check before choosing DFU or application mode

### Enter DFU update mode
1. Power on or reset the device.
2. Hold the DFU button while the device starts.
3. Keep the button pressed until the device enters DFU mode.

### Start the normal application
- Do not hold the DFU button at startup.
- The device will boot the normal application automatically.

### Summary
- Hold the button during reset to force DFU mode.
- Release the button before reset to boot the normal application.
- In some cases, the device may do a quick self-check before deciding what to do.

If you need the exact button pin, check the product documentation or the board schematic.
