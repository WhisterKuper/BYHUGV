# BYHUGV

BYHUGV Fly Controller

The repository is the main function Core firmware and supports two ways to update the firmware

* Support USB and SD card two methods to burn firmware, priority to determine whether SD card firmware exists, first rename the firmware name to 'BYHUGV.bin'
* Type 1:
* 1. The computer needs to install the DFU driver, download the DFU driver, and then install the corresponding driver according to the operating system version of your computer.
* 2. Burn this bootloader code into flight control with stlink and close the bootloader project.
* 3. Power off the flight control first, click firmware update, double-click to select the corresponding firmware (suffix.hex file), and finally plug in the flight control USB until the burning is complete.
* Type 2:
* 1. Burn this bootloader code into the flight control with stlink and close the bootloader project.
* 2. Set firmware (suffix:. Bin file) into the BYHUGV/Bootloader folder, restart the flight control. (After updating the firmware, the firmware in the SD will be automatically deleted, so that the firmware will not be updated again after the next power-on.)

Attention:

(1) PPK is the GPS raw data record

(2) The necessary sensors are RM3100 and ADIS16470

(3) GPS signals refer to the requirements for recording documents
