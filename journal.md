# 6/20
Time spent: 4h
Read through the [hardware design with rp2350](https://datasheets.raspberrypi.com/rp2350/hardware-design-with-rp2350.pdf) document, and some of the rp2350 datasheet, and got started with the design.

Since the RP2350 supports dual SPI chips, i'm looking into adding an SPI EEPROM like the AT25M02 to the design, which will allow for more flexibility with storage.

# 6/21
Time spent: 5h
I did some research into how SPI works, like the chip select pin, and how it works on the RP2350. I think I'm going to swap the RP2350**A** for the RP2350**B**, for more gpio and flexibility for on-board features. I'm probably also going create another devboard in a larger formfactor that allows breaks out ALL the pins on the RP2350**B**, and maybe some more overkill things :)
I'll probably call it either the Pico++ or the Pico Max.

I've also made the footprint for the pin headers, including the castellated pins.
![img](https://hc-cdn.hel1.your-objectstorage.com/s/v3/527646f598878c7d005d01c993580efd04e6253f_kicad_vvetgcxh3u.png)
