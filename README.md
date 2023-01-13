# Akai S1000 Project

The idea is to put all information about the Akai S1000 in 1 place...
and maybe try to recreate the S1000

The reason is simple: </br>
there is a project called Akaizer v2.4 for Windows </br>
to emulate the Time Strech algorithm of the S1000 introduced in EPROM v2.2 </br>
https://the-akaizer-project.blogspot.com/ </br>
https://drive.google.com/file/d/1gCJNSGe0BPfxVrWPJ2NzykjbzqH2iBag/view </br>
there were versions for OSX & Linux. </br>
https://akaizer.blogspot.com </br>
No WayBack archive, will upload later. </br>
https://chilloutwithbeats.com/en/akaizer-intro/ </br>

the problem with Software vs. Real S1000 Hardware, Real EPROM v2.2 </br>
is the same problem with all software: </br>
CPU vs. DSP </br>
No matter how good the code is, </br>
CPU can never have the same result, </br>
close but never the same. </br>
The reason is simple: </br>
CPU has 10 Million Interrupts per second, </br>
Audio Algorithms do Not like to be interrupted. </br>

Digital Audio is a Fast Sample & Hold,  </br>
Interrupts create another Sample & Hold on top of that Sample & Hold. </br>
also having Real AD/DA converters add analog flavor/taste/smell to digital samples.  </br>
That problem is Not as noticieable in Video, because Video goes at 30fps, 60fps, 120fps, </br>
instead audio goes at 44100, 48000, 96000 samples per second, and is played in real time, </br>
Video must be buffered in buckets to be displayed, very high speed serial, 
to very low speed parallel, but Audio cannot be buffered the same way. </br>
Some people think that processing oversampled can solve the problem, but does Not, </br>
the problem is Not frequency, is Interrupts. </br>


The idea is to keep the S1000 alive, but there are many obstacles... </br>
#1. There is No Schematics available. </br>
There are for S1100, a Cost Reduced version, </br>
but its very different in some ways... </br>
for example: </br>
the S1000 has 4x EPROMS, </br> 
the S1100 has 2. </br>
the S1000 has 1x SMPS 5v 6A = 30watt, </br>
the S1100 has dual voltage 5v and 12v SMPS. </br>
etc... </br>
#2. there are different revisions of the PCB, and the optional cards. </br>
#3. Nobody on internet has the 4x EPROMS </br>
IC09, IC10, IC11, IC12, Only 2x EPROMS IC09, IC10. </br>
S1000 Operating system can be upgraded just replacing 2x EPROMS IC9 & IC10, </br>
is Unknown what the other 2x EPROM do or how was replaced in S1100. </br>
i Have removed all Eproms i have from a S1000 and will Extract with XGecu TL866ii plus, </br>
but i have an older version of the board, came with v2.1 Eproms. </br>
Unknown if later revisions of the S1000 have a different IC11 & IC12. </br>
some machines allow to split the code different versions, and work ok. </br>
for example: Chauvet Q-Scan 250 </br>
#4. The S1000 Service Manual is very Basic, only has DC offset "Class A/B" calibration procedure for the AD/DA boards. </br>
does Not even tell what voltage to measure in the SMPS & Linear PSUs, you have to unscreq the PSU to know its a 5v 6A. </br>
take photos of the linear regulators to know the voltages for the Analog circuit. </br>
the Original Back Panel PSU / Trnasformer / Flyback or what ever it is... is Unknown. </br>

The Project RoadMap. </br>
1. Collect all information. </br>
2. Recreate all boards in KiCAd or similar, Target3001!, etc... </br>
3. Reduce Size, Replace all CMOS logic with FPGA. </br> mini Akai S1000, similar to PiAmiga and A1500 Amiga cases. 
4. design a complete SMT version. </br>
5. replace the screen with other easier to find screens,  </br>
   similar to Gotek that allows different screen types. </br>
6. improve air flow design.

The project has started long ago.. but Not Open Source, and incomplete. </br>
Example: someone in Austrailia is making 32MB RAM boards for S1000 </br>
https://www.firstpr.com.au/rwi/smem/  </br>
S1000 allows 4x 8MB or 1x 32MB. </br>
There were many 3rd party 8MB developers back in the day. </br>

32MB of RAM is plenty for a single instrument. </br>
IF want a GM, GS or XG compatible SoundFont.sf2 with all 128 instruments, </br>
is possible to find and convert many different SoundFonts available Online. </br>
older soundcards SoundBlasters and Advanced Gravis had 2MB, 4MB, 8MB soundfonts available. </br>
There is a Software that allows to Read & Write "Translate" many different formats. </br>
https://www.fmjsoft.com/awavestudio.html#main </br>

SCSI2SD project originally designed for Amiga and Macintosh computers, </br>
works for S1000, to emulate a HardDrive or scsi CD-ROM. </br>
https://www.gee-jee.net/?m=201906 </br>

The SCSI board has MB89352P + SCSI2SD </br>
there was a very nice SCSI software analyzer somewhere on the Net. </br>
https://datasheet.datasheetarchive.com/originals/distributors/Datasheets-111/DSAP0031844.pdf </br>
https://datasheet.datasheetarchive.com/originals/distributors/Datasheets-X/DSA842000-248.pdf </br>

https://web.archive.org/web/20121122034712/http://wiki.petroskoutoupis.com/index.php5?title=SCSI_Trace </br>
https://sourceforge.net/projects/scsitrace/files/ </br>

https://scsiexplorer.com/ </br>
