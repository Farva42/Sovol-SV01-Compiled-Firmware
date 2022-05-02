# Sovol-SV01-Compiled-Firmware
Firmware compiled for the SV01 stock board.
These files are provided with no warranty. They have been tested by myself but if you have things hooked up incorrectly IE your probe I am not responsible for damaged hardware.

I have included the instructions for installing the BL touch from Sovol. When you are hooking up the wires, ignore the colors and only look at the position of the wires. I have had to unpin the connectors before to correct mixed up wiring. If you flip your power and ground you can damage your mainboard or your probe.

*****Probe offsets are -33,0,+5. You need to adjust for your probe mount. With the stock Sovol mount X and Y should be pretty close. I set the Z to +5 to allow no chance of bed collision. You need to adjust this as needed, likely somewhere around -2.********

To update your firmware you need a computer connected to your printer with Cura or an Octoprint server. The included BL touch install manual from Sovol covers updating with Cura well. If you have Octoprint there is a plugin called firmware updater that works well. If you are using Octoprint you need to use "avrdude" as the flash method, "ATmega2560" as the AVR MCU and "wiring" as the AVR Programmer Type.

I have also included the config files if you wish to compile yourself. Depending on when you try to do this you might need to copy the settings into the configuration files for the current build.

All firmware and configs are done with the Marlin Bugfix branch as of May 1 2022
