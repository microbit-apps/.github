## Welcome to Micro:bit Apps!

We create applications that run on the [BBC micro:bit](https://microbit.org) 
to expand its reach in schools and out in the world.  Micro:bit apps 
often take advantage of [display shields](https://github.com/microbit-apps/display-shield) 
with a small color screen and controls, enabling features that usually require a smartphone, 
tablet, laptop or desktop. Micro:bit apps are generally portable and don't require an extra 
computer or internet connection. As the micro:bit only has 128kB of RAM and 512kB flash, 
it's a challenge to create apps for this relatively low-resource setting.

> Please note, we are NOT developing [mobile apps for the micro:bit](https://microbit.org/get-started/user-guide/mobile/),
> which are apps that generally run on iPad, iPhone or Android device and communicate over Bluetooth to a micro:bit. In
> constrast, micro:bit apps run on the micro:bit itself and can use a display shield to expand the app's I/O interface.

## Micro:bit Apps
  - [MicroData](https://github.com/microbit-apps/MicroData)
  - [MicroCode](https://github.com/microbit-apps/MicroCode)
  - [MicroMusic](https://github.com/microbit-apps/MicroMusic)

## Contributing

Coming...

## Developer Resources

We develop micro:bit apps using [Microsoft MakeCode](https://www.makecode.com) tooling.  Micro:bit apps make uses of MakeCode extensions (libraries) which provide access to display shield technology and 
user interface layers. 

### MakeCode tooling

There are three ways to develop micro:bit apps (which are MakeCode programs):

- **Recommended**: [VS Code extension for MakeCode](./vs-code.md)
- MakeCode web app
    - You must currently use https://makecode.microbit.org/beta to build a micro:bit app 
    - Load a micro:bit app into MakeCode using the Import button in the home page and selecting "Import URL".
- MakeCode CLI (compiler)
    1. Install the [MakeCode CLI](https://microsoft.github.io/pxt-mkc/).
    2. Attach a micro:bit to your computer using USB cable.
    3. Clone a micro:bit app repo and cd to it
    4. invoke `mkc -d`, which will produce the micro:bit hex file (in built/mbcodal-binary.hex) and copy it to the micro:bit drive.

### MakeCode extensions

Extensions built by this organization include:
  - https://github.com/microbit-apps/display-shield
  - https://github.com/microbit-apps/user-interface-base
  - https://github.com/microbit-apps/MicroGUI
    
### MakeCode for the micro:bit

The MakeCode web app (and related assets used by the CLI and VS Code extension) is built from:
  - https://github.com/microsoft/pxt-microbit
  - https://github.com/microsoft/pxt-common-packages
  - https://github.com/microsoft/pxt

### CODAL C++ runtime

The MakeCode compiler links the MakeCode program against
the CODAL runtime for the micro:bit, built from:
  - https://github.com/lancaster-university/codal-microbit-v2
  - https://github.com/lancaster-university/codal-nrf52
  - https://github.com/lancaster-university/codal-core

The following repo provides details on how build CODAL
  - https://github.com/lancaster-university/microbit-v2-samples
