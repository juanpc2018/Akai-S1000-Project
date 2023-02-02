L6009A5010 / 384736J1 GCMK-204X 94V-0 </br>

Dimensions: </br>
365.25mm = 14,37992125984252" Measured. </br>
365.252mm = 14,38" Aprox.</br>
x </br>
220.50mm = 8,681102362204724" Measured. </br>
220.472mm = 8,68" Aprox.</br>
x </br>
1.6000mm = 0,062992125984252" Measured. </br>
1.6002mm = 0,063" Aprox.</br>

4-Layer Board </br>
but Layer 2-3, seem to be very large planes only for (+) & GND, Unconfirmed, </br>
very large planes close to eachother seem to be emulating a Cappacitor, Unknown cappacitance. </br>
most components are on Layer-1, SMT & Throughole. </br>
most traces on Layer-4, almost all have Classic Digital Horizontal Design. </br>
Board has a 16-Bit 8088 type CPU with 7 "0-6" 64-Pin Nubus like connectors, </br> 
9-port 8-Bit Super i/o expander, soldered Async SIMM CPU RAM, SRAM </br> 
upto 32MB Sound/Sample Memory add-on card(s) SIMM, similar to 72-Pin RAM. </br>
Built-In MIDI i/o connectors, Floppy controller, 640x240 LCD HD44780 type Screen, </br>
optional add-on cards: Digital Audio i/o board, SCSI controller board. </br>
IC9, IC10, IC11, IC12 UV-C Eraseable EPROMS 27C512, "2x Unknown purpose", </br>
XO: </br>
2x 16MHz, </br>
1x 33.8688MHz TD3080/TD11000 </br> 

IC1 NEC µD70216GP-8 V50 1984 CPU / MCU </br>
IC2 TEL TE7730 Super i/o </br>
IC3 L7A0218 / FLR-6009 / 8902 Unknown, </br>
IC4 L7A0109 / ITP-6009 / 8851 Unknown. </br>
IC5 LC7981 LCD Screen </br>
IC6 NEC D7265C Floppy </br>
IC7 NEC D71065G Floppy </br>
IC8 NEC MB89255A Parallel io </br>
IC13 Sony CXK5816PN-12L SRAM </br>
IC14 MN41464A-08 </br>
IC15 " </br>
IC16 " </br>
IC17 " </br>
IC18 74ac158e </br>
IC19 " </br>
IC20 74hc138p </br>
IC21 74hc259p </br>
IC22 74hc365p </br>
IC23 74hc393p </br>
IC24 74hc195p </br>
IC25 74hc279p </br>
IC26 74hc139p </br>
IC27 74hc74p </br>
IC28 74hc595p </br>
IC29 74hc595p </br>
IC30 74hc573p </br>
IC31 74hc573p </br>
IC32 74act573e </br>
IC33 74ac139e </br>
IC34 74ac541e </br>
IC35 " </br>
IC36 74hc14p </br>
IC37 74hc04p </br>
IC38 74hc08p </br>
IC39 74ac04e </br>
IC40 74ac00e </br>
IC41 74ac32e </br>
IC42 74hc10p </br>
IC43 74hc04p </br>
IC44 74hc00p </br>
IC45 74hc32p </br>
IC46 74hc08p </br>
IC47 9L T520D </br>
IC48 78M12 </br>
IC49 79M12 </br>
IC50 MN41464A </br>
IC51 " </br>
IC52 " </br>
IC53 " </br>
IC54 74ac139e </br>
IC55 74hc32p </br>
P108 34-Pin Floppy Controller </br>
P109 26-Pin Front Panel </br>
P110 50-Pin Ribbon </br>
P112 10-Pin Front Panel </br>
P114 Back-Light </br>
P117 </br>
P118 4-Pin Floppy Power connector. </br>
P119 </br>
P111 5vdc 6A </br>
P115 12-0-12 AC Power Input </br>
J101 MIDI In/Out/Thru </br>
IC47 9L T520D </br>

Scanning The Bottom Layer-4 on a Cheap scanner with RGB-LED + Monochromatic CCD </br>
Scanner moves Vertical, Scans Horizontal PCB traces flawless, </br>
but Vertical PCB traces are invisible, because the light angle/polarity/phase. </br>
45° Traces are 25%-50% visible. </br>
probably PCB scanning requires a White Source + RGB CCD sensor "The opposite technology". </br>

Weird things: </br>
cutting traces on Layer-4 to install more than 2MB sample memory. </br>
Headphone output pcb is on the Back of the Chasis, over the Regulators Heatsink,</br>
but MainPCB connector is on the Front of the case, with a long cable. </br>
Crazy design / Things to improve. </br>

The linear Regulators +12/-12vdc on the MainPCB, </br>
is an independent circuit on the MainPCB, but some traces go somewhere, Voltage Drop & Current limited with Diodes. </br>
dropped voltage goes somewhere, probably to Headphone output circuit on the ther side of the MainPCB. </br>
Analog Audio PCB i/o PCB is appart, connected with a 50-pin ribbon cable, and another 3-pin for +12/-12dc.</br>  
Analog PCB should be +15/-15vdc, or best case +18/-18vdc, </br>

The +12/-12 Linear Voltage Regulators, Diode Bridge, AC-AC Transformer can be Replaced with: </br>
2x SMPS MeanWell RS-25-12 "12v 25w 2A" or similar + 2x large >2200µF 25v. </br>
or </br>
2x SMPS MeanWell RS-25-15 "15v 25w 1.6A" or similar </br>
RS-15-xx too small. </br>
RS-50-xx too Big. </br>
RD-3513 is an option, 13.5vdc 1.3A 35w/2=17.5w "Barelly works" adjustable: 11.5v-15.5v </br>
