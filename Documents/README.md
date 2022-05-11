# STMicroelectronics NUCLEO-G0B1RE

## Overview

The STM32 Nucleo-64 board provides an affordable and flexible way for users to try out new concepts and build prototypes by choosing from the various combinations of performance and power consumption features, provided by the STM32 microcontroller. For the compatible boards, the external SMPS significantly reduces power consumption in Run mode. The ARDUINO® Uno V3 connectivity support and the ST morpho headers allow the easy expansion of the functionality of the STM32 Nucleo open development platform with a wide choice of specialized shields.

## Documentation

- [NUCLEO-64 user manual](https://www.st.com/resource/en/user_manual/um2324-stm32-nucleo64-boards-mb1360-stmicroelectronics.pdf)
- [NUCLEO-G0B1RE data brief](https://www.st.com/resource/en/data_brief/nucleo-g0b1re.pdf)

## CMSIS-Drivers

This board support pack contains a CMSIS-Driver for the [VIO](https://arm-software.github.io/CMSIS_5/develop/Driver/html/group__vio__interface__gr.html) interface. This is a virtual I/O abstraction for peripherals that are typically used in example projects. The **Blinky** example uses this interface to create a blinking light with the USER LED mounted on the board that can be controlled by the **Button USER**.

Virtual Resource  | Variable       | Physical Resource on NUCLEO-G0B1RE             |
:-----------------|:---------------|:-----------------------------------------------|
vioBUTTON0        | vioSignalIn.0  | GPIO C.13: Button USER                         |
vioLED0           | vioSignalOut.0 | GPIO A.5:  LD2 GREEN                           |

## ST-LINK driver installation and firmware upgrade

1. Download the latest [ST-LINK driver](https://www.st.com/en/development-tools/stsw-link009.html) (Windows only).
2. Extract the archive and run `dpinst_amd64.exe`. Follow the displayed instructions.
3. Download the latest [ST-LINK firmware upgrade](https://www.st.com/en/development-tools/stsw-link007.html) (Linux/Mac OS/Windows).
4. Extract the archive and run the STLinkUpgrade application.
5. Connect the board to your PC using a USB cable and wait until the USB enumeration is completed.
6. In the **ST-Link Upgrade** program, press the **Device Connect** button.
7. The current ST-LINK version should be displayed.
8. Press the **Yes >>>>** button to start the firmware upgrade process.

## Technical references

- [STM32G0B1RE microcontroller](https://www.st.com/en/microcontrollers-microprocessors/stm32g0b1re.html)
- [NUCLEO-G0B1RE](https://www.st.com/en/evaluation-tools/nucleo-g0b1re.html)
