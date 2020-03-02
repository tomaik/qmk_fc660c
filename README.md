# How to install:

## Clone qmk_firmare repository

```sh
git clone --recurse-submodules https://github.com/qmk/qmk_firmware.git
cd qmk_firmware
```

## Install build dependencies:

- Fedora:

```sh
sudo dnf install dfu-util dfu-programmer avr-gcc avr-libc binutils-avr32-linux-gnu arm-none-eabi-gcc-cs arm-none-eabi-binutils-cs arm-none-eabi-newlib
```

## Verify build (from root qmk dir)

```sh
sudo make fc660c:default (or other keymap name)
```

## Install

```sh
sudo make fc660c:tomaik:dfu
```

click reset button on keyboard and wait

## Extra

Create layout using [qmk web configurator](https://config.qmk.fm).

Example: [tomaik.json](tomaik.json)
