Total Time Spent: 39h

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

# 6/22
Time spent: 4h
Finished the schematic design, and looked at the pico 2 source schematic to see if I made any errors. I've also sourced most of the parts on LCSC. The preliminary cost is about $120 USD (ENIG + Standard PCBA)

# 6/23
Time spent: 1h
Added SWD debug pads to the design. I've also started working on the PCB layout and routing.
![img](https://hc-cdn.hel1.your-objectstorage.com/s/v3/57cf6244f8e609582fa10e30bc9018dc36da321c_kicad_hx3xjgqanx.png)
![img](https://hc-cdn.hel1.your-objectstorage.com/s/v3/00b9f7523d85120827689f38e826afcdeeb987b4_kicad_t2y2yx98e9.png)

# 6/24
Time spent: 7h
Sat at my desk and made some tweaks to the schematic- the I2C EEPROM chip was removed because there just wasn't enough space on the board, and it costs quite a bit. I then decided to delete all traces and vias and start again. I've fully routed the board in a couple hours.
![img](https://hc-cdn.hel1.your-objectstorage.com/s/v3/f21e9aa79d16d40aaa7a059a5c4ab1665984f3c9_kicad_pemno1jvuh.png)

# 6/25

--
Time spent: 6h
Did this all in a couple hours at a coffee shop. I redid the power layout and finished the PCB. On to sourcing parts now![img](https://hc-cdn.hel1.your-objectstorage.com/s/v3/4195242a2c4d129d6ec4d91fcfe52e4d6db890c9_kicad_tyf9tc7nlb.png)
--

--
Time spent: 4h
Redid and moved around a bit of the power supply, and then optimized the BOM and things for PCBA. I then realized the project would be overbudget, so I decided to get a hotplate and reflow the parts myself, which is much cheaper. I then created the master BOM for LCSC and JLCPCB.
I decided to get the hotplate off amazon as the price is only $1 more than AliExpress.


# 7/9

Time spent: 5h

The parts arrived and I reflowed the pcb, it works!
PS. 0201 components are HELLLISH to deal with

![20250802_234625](https://github.com/user-attachments/assets/ac3c3b91-a325-455c-a22e-cf02540d6588)
![20250802_234557](https://github.com/user-attachments/assets/fb6c73b7-ecd5-4205-883c-76b04d625d86)
![20250709_195919](https://github.com/user-attachments/assets/6b623a33-3bf1-47d3-888f-86e763c83936)
