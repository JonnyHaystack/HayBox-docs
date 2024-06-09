# Installation

If you want to simply use a pre-built firmware with default pin mappings and configuration, refer to the [pre-built binaries](#pre-built-binaries) section. If you want to make any changes to the code, refer to the [building from source](#building-from-source) section.

1. Browse the [existing configs](config/) to determine which config is appropriate for your hardware
2. Download the corresponding artifact from either the [latest HayBox release](https://github.com/JonnyHaystack/HayBox/releases), or from a [workflow run](https://github.com/JonnyHaystack/HayBox/actions) if you want the latest development version (unstable).
3. Flash the firmware to your microcontroller in the usual way
   - If you are using a Pico/RP2040 build (`.uf2` file), simply put it into bootsel mode while plugging it into your PC, and drag and drop the `.uf2` file onto the RPI-RP2 drive that comes up
   - If you are using Arduino/AVR build (`.hex` file), you can use a program like [QMK Toolbox](https://github.com/qmk/qmk_toolbox) to flash the `.hex` file to it