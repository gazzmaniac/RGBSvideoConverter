# RGBSvideoConverter
RGB to SVideo converter for Amiga computers

I have decided to opensource the Red Keg Retro RGB to SVideo converter.
Licensed under the TAPR Open Hardware License (www.tapr.org/OHL)
Please be aware that some of the footprints may not be open source even though they are public domain.

This device is based around the AD723ARUZ PAL encoder.  It converts 15 kHz RGB signal to SVideo and Composite.  It is designed for and tested with the Amiga series of computers however it should work with other machines that output a 15 kHz RGB signal.  The circuit is substantially based on the examples given in the AD732ARUZ data sheet.

The video input is via a D9 socket with the same pinout as the Commodore 1084 monitor (except csync is not used) and power is 3.3-5v into a 5 mm DC power socket.  Power may be supplied from the Amiga.  A suitable cable would be:
AmigaD23 AdapterD9  AdapterPower   Signal
  16-20    1,2         sleeve       GND
    3       3                       Red
    4       4                       Green
    5       5                       Blue
    11      8                       HSync
    12      9                       VSync
    23                  pin         +5V

This project has been built and tested however no warranty is given.

Notes:
JP1 selects whether or not the YTrap filter is used.  There is no need to remove this.


Rev 1.1:
First open source release.
The only changes are in the silkscreens to reflect the now open nature of the project.
