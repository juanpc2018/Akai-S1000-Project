The Screen is a Hitachi LM200 240x64 110x30mm, 140x40mm frame, </br>
controller is Not on the Screen, like most screens </br>
Hitachi HD44780 compatible, like Sitronix ST7920 </br>
Akai S1000 has Sanyo LC7981 | 8F2 controller IC, </br>
Sony CXK5816PN-12L Memory.</br>

There are 3 options: </br>
A) replace the backlight of the original screen, slide-in </br>
with a cellphone backlight, and cut to proper size. </br>

B) replace the whole screen with a New compatible LM200 LED or OLED. </br>
Positive or Negative "Dark Background, White Letters". </br>

C) replace with incompatible screen. </br>

Method A) is the most economical & easy. </br>
but visually Not the best, </br>
Original/Old screen has a pale washed Cyan color, Not the most pleasing. </br>

Method B) $120usd + shipping. </br>
LM200 screen is similar for: </br>
Akai MPC 3000 </br>
Akai MPC 60 mkII </br>
S-series samplers require different pin / ribbon connector.  </br>
Akai S1000 </br>
Akai S1100 </br>
Akai S2800 </br>
Akai CD3000 CD3000XL CD3000i </br>
Akai S3000 </br>
Akai S3000XL </br>
Akai S3200 </br>
Akai S3200XL </br>
Akai VX600 </br>

New LED Screen = NO NEED for Inverter. </br>
simple installation (No soldering required). </br>

Method C) is the most complicated, </br>
There is 3 ways to do it, </br>
1. Translate signals coming from 10-pin connector,</br>
from Sanyo LC controller out with a micro like ATmega, FPGA or similar, </br>
Screen refresh is around 500kHz. </br>
this is the less invasive method. </br>

2. Best invasive option: </br>
desolder the Sanyo LC ocontroller, </br>
emulate the controller with a micro ATmega2560, FPGA or similar, </br>
Read signals coming from the Nec v50 "8088" CPU and 16-Bit multiplexer TEL TE7730 | 8926 Z78 </br>
translate LC7981 Byte instructions to other graphical screen controller instructions. </br>

3. Modify the S1000 ROM Firmware to replace Sanyo LC7981 bytes to other like T6963C, RA6963, ST75256P. </br>

There are many different sceens today, for PI and Arduino. </br>
some graphical, some fixed characters, </br>
Example: </br>
SSD1306 0.96" </br>
has 128x64, using 2 screens Side-by-Side = 256x64 </br>
screens work in i2c or ISP mode, but... </br>
SSD1306 are tiny small, miniature, micro size. </br>
thats miniaturizing too much. </br>
sister screen: </br>
SH1106 is a bit bigger 1.3" x2 but still very small. </br>

Adafruit-4393 miniPiTFT 1.14" 240x135, smaller.  </br>

Same Jumbo Pixel Size: </br>
LGM240128A-NSW-BBW with Toshiba T6963C controller. </br>
that screen is 240x128, Not 240x64. </br>
64 pixels must be unused, empty, 32 top, 32 bottom to center the image, </br>
or 64 empty at the bottom, to fit the screen in the S1000 chasis, requires standoffs. </br>

There is also a Jumbo screen 128x64 with ST7920. </br>
Requires 2x like the smaller, but edge are bigger, very visible. </br>

there are 2.8" | 3.2" and 3.5" </br>
2.8" Adafruit-1601 PiTFT 320x240 TFT+Touchscreen Pi </br>
3.2" </br>
TFT320QVT 3.2″ 320×240 3.3vdc ILI9341 | touch ic: XPT2046 </br>
3.5" </br>
MPI3501 320x480 XPT2046 Pi </br>
MAR3513 320x480 ILI9486/ILI9488 Arduino Mega2560 pin compatible. </br>

looking all screens side by side, 3.5" seems the minimum size, </br>
or same pixel size. </br>
miniature screen could be fun, but Not a long term sollution, </br>
unless you have a magnifier lens infront, to see from far. </br>

4. Last option is to create a VGA output: </br>
RGBHV signal 320x240, must be compatible with modern / cheap VGA to HDMI converters. </br>
