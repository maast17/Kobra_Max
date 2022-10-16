How to install

Go to your printer -> Settings -> About -> Firmware Version -> check your current version
Grab an empty SD card and drop the firmware.bin on it
Put the SD card in the printer and boot it. The printer will be stuck on the end of the splash screen, don't do anything and wait until the menu appears
When the menu appears, go back to About and check your firmware version again, you should see jojos38 edited Kobra Vx.x.x
Connect your printer to your PC and run the following commands in the same order: M710 A1 I4 S5 M500 (This makes the motherboard's fan more silent)


Features

Faster auto leveling
Faster homing
Reduced noise (motherboard fan)
Linear Advance enabled
SQUARE_WAVE_STEPPING enabled
TMC_ADV enabled/modified:
TMC_ADV() { \
    stepperX.dedge(true); \
    stepperY.dedge(true); \
    stepperZ.dedge(true); \
    stepperE0.dedge(true); \
   }


Compile instructions

Follow the guide on https://www.reddit.com/r/anycubic/comments/y2waxu/tutorial_how_to_build_anycubic_marlin_source_code/
