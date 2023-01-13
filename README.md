# Akai S1000 Project

The idea is to put all information about Akai S1000 in 1 place...
and maybe try to recreate the S1000

The reason is simple: </br>
there is a project called Akaizer v2.4 for Windows </br>
to emulate the Time Strech algorithm of the S1000 from EPROM v2.2 </br>
https://the-akaizer-project.blogspot.com/ </br>
https://drive.google.com/file/d/1gCJNSGe0BPfxVrWPJ2NzykjbzqH2iBag/view </br>

there was versions for OSX & Linux. </br>
https://akaizer.blogspot.com </br>
No WayBack archive, i will upload later. </br>

the problem with that software vs. Real S1000 Hardware, Real EPROM v2.2 </br>
is: CPU vs. DSP </br>
No matter how good the code is, </br>
CPU can never have the same result of DSP, close but never the same. </br>
The reason is simple, CPU has 10Million Interrupts per second, Audio Algorithms do Not like to be interrupted. </br>
also having real AD/DA converters adds analog flavor/smell to digital samples.  </br>

The idea is to keep the S1000 alive, but there are many obstacles... </br>
#1. There is No Schematics available. </br>
There are for S1100 a Cost Reduced version, </br>
but its very different in some ways... </br>
for example: </br>
the S1000 has 4x EPROMS, the S1100 has 2. </br>
the S1000 has 1x SMPS 5v 6A = 30watt, </br>
the S1100 has dual voltage 5v and 12v SMPS. </br>
etc... </br>
#2. there are different revisions of the board PCB, and the optional cards. </br>
#3. Nobody on internet has the 4x EPROMS: </br>
IC09, IC10, IC11, IC12, Only 2x EPROMS IC09, IC10. </br>
S1000 Operating system can be upgraded just replacing 2x EPROMS IC9 & IC10, </br>
is Unknown what the other 2x EPROM do or how was replaced in S1100. </br>
i Have removed all Eproms i have from a Real S1000 and will Extract with XGecu TL866ii plus, </br>
but i have an older version of the board that came with v2.1 Eproms. </br>
Unknown if later revisions of the S1000 have a different IC11 & IC12. </br>


