The Screen is a Hitachi LM200 240x64 110x30mm Screen, 140x40mm frame, </br>
controlleer is Not on the Screen, like most screens </br>
Hitachi HD44780 compatible, 
Akai S1000 has Sanyo LC7981 8F2 controller IC, </br>
Sony CXK5816PN-12L Memory.</br>

There are 3 options: </br>
A) replace the backlight of the original screen, its a slide card </br>
with a cellphone backlight, and cut to proper size. </br>

B) replace the whole screen with a New compatible LM200 LED or OLED. </br>
Positive or Negative "Dark Background, White Letters". </br>

C) replace with other incompatible screen. </br>

Method A) is the most economical & easy. </br>

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
simple installation (no soldering required). </br>

Method C) is the most complicated, </br>
There is 2 ways to do it, </br>
1. Translate signals coming from 10-pin connector,</br>
Sanyo LC controller with a micro like ATMega or similar, </br>
Screen refresh is around 500kHz. </br>

2. Best option: remoce the Sanyo LC ocontroller, </br>
emulate the controller with a micro ATmega2560 or similar, </br>
Read signals coming from the Nec v50 CPU and 16-Bit multiplexer TEL TE7730 8926 Z78 </br>
translate Byte instructions for LC7981, to other graphicak screen instructions. </br>

There are many different sceens on the market today, for PI and Arduino </br>
some graphical, some fixed characters </br>
Example: </br>
SSD1306 0.96" </br>
-SH1106 
