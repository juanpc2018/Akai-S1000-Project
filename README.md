# Akai S1000 Project 
###### v1.00000001
-----------

The idea is to put all information about the Akai S1000 in 1 place...
and maybe try to recreate the S1000

The reason is simple: </br>
there is a project called Akaizer v2.4 for Windows </br>
to emulate the Time Strech algorithm of the S1000 introduced in EPROM v2.2 </br>
https://the-akaizer-project.blogspot.com/ </br>

the problem with Software vs. Real S1000 Hardware, Real EPROM v2.2 </br>
is the same problem with all software: </br>
CPU vs. DSP </br>
No matter how good the code is, </br>
SW can never have the same result, </br>
close but never the same. </br>
The reasons are simple: </br>
Modern CPU has 10 Million Interrupts per second, </br>
Audio Algorithms do Not like to be interrupted. </br>
L1/L2/L3 cache is Not Big Enough for a modern OS, </br>
Modern CPU's have Branch Prediction algorithms </br>
predictions are used to "fake" increase speed by guessing the result before result is computed </br>
but predictions can never be 100% accurate, and millions of predictions per second, affect sound. </br>
There is something lost, distorted in the process, makes sound plastic / artificial. </br> 

Digital Audio is a Serial Sample & Hold,  </br>
Interrupts create another Sample & Hold on top of that Sample & Hold. </br>
having Real AD/DA converters add analog flavor/taste/smell to digital.  </br>
That problem is Not noticieable in Video, because Video goes at 24fps, 30fps, 60fps, 120fps, 240fps. </br>
instead audio goes at 44100, 48000, 96000 samples per second, and is played in real time, </br>
Video must be buffered in buckets to be displayed, very high speed serial, </br>
to very low speed parallel, but Audio cannot be buffered the same way. </br>
Some people think that processing with Oversampling can solve the problem, but does Not, </br>
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
is unknown what the other 2x EPROM do or how was replaced in S1100. </br>
removed all Eproms i have from a S1000 and Extract with XGecu TL866ii plus, </br>
S1000 was manufactured between 1988 to 1993, the board i have came with v2.1 Eproms. </br>
Unknown if later revisions of the S1000 have a different IC11 & IC12. </br>
some machines allow to split the code in different versions and work ok. </br>
example: Chauvet Q-Scan 250 </br>
#4. The S1000 Service Manual is very Basic, only has DC offset "Class A/B" calibration procedure for the AD/DA boards, </br>
does Not even tell what voltage to measure in the SMPS & Linear PSUs, you have to unscrew the PSU to know its a 5v 6A, </br>
take photos of the linear regulators to know the voltages for the Analog circuit. </br>
the Original Back Panel PSU / Transformer / Flyback / Inverter... is Unknown. </br>

The Project RoadMap: </br>
1. Collect all information. </br>
2. Recreate all boards in KiCad or similar: Target3001!, etc... </br>
3. Reduce Size, Replace all CMOS logic with FPGA or micros. </br> 
mini Akai S1000, similar to PiAmiga and A1500 Amiga cases. </br>
4. design a complete SMT version. </br>
5. replace hard to find components with easy to find components, like the screen, </br>
   similar to Gotek that allows different screen types. </br>
6. improve air flow design with thermal camera.

The project started long ago.. but Not Open Source, and incomplete. </br>
Example: someone in Australia is making 32MB RAM boards for S1000 </br>
https://www.firstpr.com.au/rwi/smem/  </br>
S1000 allows 4x 8MB or 1x 32MB. </br>
There were many 3rd party 8MB developers in the 90s, </br>
most used different chipset, some had resistor networks, capacitors, others Not, </br>
some had electrolitics, others tantalum, some branded, some generic. </br>
i have a 8MB Generic 4-layer PCB, </br>
16x Ti TMS44100DJ PCP 4063 IN -80 </br>
2x 74HC541 </br>
2x 74AC541 </br>
3x Res Net 4-101GB </br> 

32MB of RAM is plenty for a single instrument. </br>
A) download a very large SoundFont like: Musyng Kite.sf2 and split the instruments, </br>
B) IF want a complete GM, GS or XG compatible SoundFont.sf2 with all 128 instruments + Drums </br>
is possible to find and convert many different SoundFonts available Online. </br>
older soundcards Sound Blasters and Advanced Gravis had 2MB, 4MB, 8MB upto 32MB soundfonts available. </br>
some better than others... some 8MB were better than some 32MB, </br>
here some .SF2 examples: </br>
http://www.arachnosoft.com/main/soundfont.php </br>
https://www.vogons.org/viewtopic.php?p=707079 </br>
https://www.reasonbanks.com/refill_proVitamin_demo.html </br>
https://musical-artifacts.com/artifacts/538 </br>
http://ntonyx.com/sf_f.htm </br>
https://ia601004.us.archive.org/4/items/soundfonts_201910/8mbgm_enhanced18.sf2 </br>
https://archive.org/download/500-soundfonts-full-gm-sets </br>

The 8x Akai S-series CD-ROMs, the 8th has different GM versions, </br>
havent tested vs. popular GM.sf2 on the net. </br>

Some people Remember Old Games MIDI music in a certain way, others in other way, different Guitars, MT-32, FM, CZ-101 </br>
There are many DOOM, Sierra & Prince of Persia Sound Tests online. </br>

Software that allows to Read & Write & "Translate" different formats. </br>
https://sourceforge.net/projects/akaiutil/files/ </br>
https://www.fmjsoft.com/awavestudio.html#main </br>
http://www.chickensys.com/translator/documentation/formatinfo/akai.html </br>
http://www.chickensys.com/products2/software.html </br>
http://www.soundlib.com/cdxtract/ </br>
https://samplerzone.com/products/millennium </br>
https://archive.org/search.php?query=Akai+s1000 </br>
https://archive.org/details/mesa_20210818 </br>
http://oldschooldaw.com/forums/index.php?topic=2631.0 </br>
http://web.archive.org/web/20000303000424/http://www.akaipro.com/software-MESAmac.html </br>
http://web.archive.org/web/20000303013504/http://www.akaipro.com/software-MESApc.html </br>
https://www.kvraudio.com/forum/viewtopic.php?t=229457 </br>
https://web.archive.org/web/20070403104457/http://www.akaipro.com/archive_os/mesa2v2.zip </br>
http://web.archive.org/web/20000817005312/http://www.akaipro.com/downloads.html </br>
https://web.archive.org/web/20131010213139/http://www.hollowsun.com/gagnon/download/archive_om.html </br>
http://macos9lives.com/smforum/index.php?topic=1255.msg15243#msg15243 </br>
https://web.archive.org/web/20131205074601/http://www.hollowsun.com/gagnon/download/aks_dload.html </br>
https://akais3000.wordpress.com/2010/01/01/mesa-akai-sample-editor/ </br>
http://macos9lives.com/smforum/index.php?topic=1255.0 </br>

