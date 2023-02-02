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
Board has a 16-Bit 8088 type CPU with 64-Pin Nubus like connectors, 9-port 8-Bit Super i/o expander, </br>
soldered Async SIMM CPU RAM, upto 32MB add-on card(s) SIMM SampleRAM, similar to 72-Pin RAM. </br>
Built-In MIDI i/o connectors, Floppy controller, 640x240 LCD HD44780 type Screen, </br>
optional add-on cards: Digital Audio i/o board, SCSI controller board. </br>
4x UV-C Eresable EPROMS, 2x Unknown purpose. </br>

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
