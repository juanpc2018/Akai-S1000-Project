Screen is a Hitachi LM200 240x64 pixels with HD44104 driver IC</br>
180x75mm PCB, </br>
132x39mm screen, </br>
127x34mm pixel area, </br>
1.6mm pcb, 4.5~6.0mm front depth </br>
controller is Not on the Screen, like most screens. </br>

LM213B 256x64 is the only with built-in controller from that era. </br>
LM215 480x128 Bigger. </br>

LM200 was designed for Hitachi HD61830 control LSI, </br>
Not the common HD44780, like Sitronix ST7920 </br>
but... </br>
Akai S1000 has Sanyo LC7981 control LSI, </br>
Sony CXK5816PN-12L Memory.</br>

Akai S1000 display circuit is similar to CB1020R. </br>
Hitachi HD61830 developer boards: </br>
"Control Circuit Board" CB-Series:  </br>
CB1020R, CB1026R, CB1030R. </br>

------

There are 3 options: </br>
A) Replace the backlight of the original screen, slide-in </br>
with a cellphone backlight, and cut to proper size. </br>

B) Replace the whole screen with a New LM200 compatible LED or OLED, </br>
10-pin version = No LC7981 Controller built-in,  </br>
Positive "Blue/White" or Negative "Dark/White". </br>

C) Replace Original screen with incompatible screen. </br>

Method A) the most economical & easy. </br>
but visually Not the best, </br>
Old screen has a pale washed Cyan color, Not the most pleasing. </br>

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

New LED Screen = No Inverter. </br>
simple installation ("No soldering"). </br>

This is Not a long term sollution if New 10-pin compatible screens are No longer manufactured. </br>
price is already double vs. similar 240x64 screen. </br>

Method C) most complicated, </br>
There are 3 ways to do it, </br>
1. Less invasive method:
Translate signals coming from 10-pin connector,</br>
from Sanyo LC7981 with a micro like ATmega, FPGA, STM32 or similar, </br>
Screen clock is around ~500kHz. </br>
Convert to other graphical screen instructions D0-D7. </br>
Not a long term sollution if LC7981 on the S1000 Fail. </br>

2. Invasive method: </br>
Desolder LC7981 on the S1000 </br>
A) Replace screen with built-in LC7981 compaticle controller. </br>
B) Emulate LC7981 with micro: ATmega2560, FPGA, STM32 or similar.. </br>
Read signals from Nec v50 "80186" CPU and 16-Bit multiplexer TEL TE7730 </br>
Translate LC7981 type signals to other graphical screen controller. </br>
C) Modify Akai S1000 ROM Firmware to replace Sanyo LC7981 to other like T6963C, RA6963, ST75256P, SSD1322. </br>

3. Create a VGA output 60Hz or Compositre, Component YPbPr, Y-C SuperVideo, </btr>
480i/p 50Hz / 60Hz or </br>
RGBHV signal 320x240 </br>
VGA must be compatible with modern / cheap VGA to HDMI converters, </br>
from 10-pin signal or emulated LC7981 or modified Akai ROM. </br>

There are many different sceens today, for Pi and Arduino. </br>
some graphical, some fixed characters, </br>
Example: </br>
SSD1306 0.96" </br>
has 128x64, using 2 screens Side-by-Side = 256x64 </br>
screens work in i2c or ISP mode, but... </br>
SSD1306 are tiny small, miniature, micro size. </br>
thats miniaturizing too much. </br>
sister screen: </br>
SH1106 is 1.3" x2 bigger but still small. </br>
ther is a bigger 2.42" hard to find. <br>
Adafruit-4393 miniPiTFT 1.14" 240x135, smaller.  </br>

Same Jumbo Pixel Size: </br>
LGM240128A-NSW-BBW with Toshiba T6963C controller. </br>
that screen is 240x128, Not 240x64. </br>
64 pixels must be unused, empty, 32 top, 32 bottom to center the image, </br>
or 64 empty at the bottom, to fit the screen in the S1000 chasis, requires standoffs. </br>

There is also a Jumbo screen 128x64 with ST7920. </br>
Requires 2x like the smaller, but screen edge is big, very visible. </br>

there are 2.8" | 3.2" and 3.5" </br>
2.8" Adafruit-1601 PiTFT 320x240 TFT+Touchscreen Pi </br>
3.2" </br>
TFT320QVT 3.2″ 320×240 3.3vdc ILI9341 | touch ic: XPT2046 </br>
3.5" </br>
MPI3501 320x480 XPT2046 Pi </br>
MAR3513 320x480 ILI9486/ILI9488 Arduino Mega2560 pin compatible. </br>

looking all screens side-by-side, 3.5" seems ok size, </br>
or smaller + fresnel magnifier lens, or same pixel size. </br>
miniature screen could be fun, </br>
with a magnifier fresnel lens in front, to see from far. </br>

There is a Wide screeen 256x64 [SSD1322](https://support.newhavendisplay.com/hc/en-us/articles/4414477846679-SSD1322) controller </br>
2.8" [NHD-2.8-25664UCB2](https://newhavendisplay.com/2-8-inch-blue-graphic-oled-module/) Blue </br>
3.12" [NHD-3.12-25664UCB2](https://newhavendisplay.com/3-12-inch-blue-graphic-oled-module/) Blue </br>
3.12" [NHD-3.12-25664UCW2](https://newhavendisplay.com/3-12-inch-white-graphic-oled-module/) White </br>
other similar brands have the connector on the side, Not on the Top. </br>
