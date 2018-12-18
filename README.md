# bluepill-bootloader
bluepill-bootloader is an open-source MakeCode UF2 USB bootloader for STM32 Blue Pill devices.

See https://medium.com/@ly.lee/stm32-blue-pill-usb-bootloader-how-i-fixed-the-usb-storage-serial-dfu-and-webusb-interfaces-36d7fe245b5c

https://medium.com/@ly.lee/work-in-progress-stm32-blue-pill-visual-programming-with-makecode-codal-and-libopencm3-422d308f252e

WebUSB and WinUSB implementation from https://github.com/trezor/trezor-mcu

USB CDC implementation from https://github.com/Apress/Beg-STM32-Devel-FreeRTOS-libopencm3-GCC/blob/master/rtos/usbcdcdemo/usbcdc.c

USB MSC patch from https://habr.com/company/thirdpin/blog/304924/

HF2 implementation from https://github.com/mmoskal/uf2-stm32f

## Build instructions


    git clone --recurse-submodules https://github.com/lupyuen/bluepill-bootloader
    cd bluepill-bootloader

Launch Visual Studio Code.

Install the PlatformIO extension for Visual Studio Code.

Open the workspace file in the above folder.

Build the bootloader and firmware.

Flash the bootloader to Blue Pill via ST-Link 2.

Copy firmware.uf2 to the USB drive exposed by the bootloader.

More details: https://github.com/mmoskal/uf2-stm32f103/blob/master/README.md

## Licensing
All contents of the project are licensed under terms that are compatible with the terms of the GNU Lesser General Public License version 3.

Non-libopencm3 related portions of the dapboot project are licensed under the less restrictive ISC license, except where otherwise specified in the headers of specific files.

See the LICENSE file for full details.
