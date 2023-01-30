SCSI add-on card for S1000 has External 50pin Centronics and internal 50-pin ribbon. </br>
External SCSI is Not required unless want to add an external SCSI CD-ROM "Obsolete", </br>
or an external SCSI2SD v5, RaSCSI, BlueSCSI, ZuluSCSI or similar that can load .iso CD-ROM images. </br>
https://github.com/guinguin-instruments/Akai-Iso-2-SD

Default SCSI card has External Connector, No Internal connector, but times change. </br>
SCSI2SD project & others designed for Amiga, Atari and Macintosh computers, </br>
work for S1000 to emulate a HardDrive or scsi CD-ROM. </br>
https://www.gee-jee.net/?m=201906 </br>
problem of this: </br>
replacing Floppy Drive with Gotek or HxC,
and adding an internal SCSI2SD, is removing the Digital i/o board. </br>
using external SCSI2SD or drilling a holes in the chassis is required to keep the Digital i/o board. </br> 
other option is to forget about Gotek / HxC and place the SCSI2SD in the floppy bay, to keep the Digital i/o board. </br>
3rd option is to fit both PCBs in the same floppy bay with a 3D printed bracket. </br>

Information about SCSI connectors is getting hard to find.. </br>
Found 2: </br>
Amphenol and TE </br>
Amphenol had different models, most were designed for bracket mount,  </br>
SCSI Centronics Secure Ears / Holders are Not on the connector, but the Bracket. </br>
TE has the connector with Secure Ears in the connector it self. </br>
The -480 model has Bracket included. </br>
https://www.connectorpeople.com/Connector/AMPHENOL/5/57-BC50B-AM100-480 </br>

The Original S1000 SCSI card has a TE type connector with a Bracket type mount "weird". </br>
if you pull the scsi cable very hard, the force will destroy the connector/card or S1000 board. </br>
The metallic chassis is Not holding the connector in the original design. </br>
Using an Amphenol type connector, to secure the connector to bracket and chassis is the proper way. </br>
The Original SCSI card is designed "to fail" in case of an accident, </br>
probably CEO decision to buy a cheaper connector. </br>

The SCSI S1000 has MB89352P </br>
but the goal is to replace that with FPGA. </br>
there were nice SCSI software analyzer on the Net. </br>
https://web.archive.org/web/20121122034712/http://wiki.petroskoutoupis.com/index.php5?title=SCSI_Trace </br>
https://sourceforge.net/projects/scsitrace/files/ </br>
https://scsiexplorer.com/ </br>
