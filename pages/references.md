# Useful References and Stuff

Some links to people and files that have helped along the way.

Original Hackaday article: https://hackaday.com/2013/01/11/ask-hackaday-we-might-have-some-fpgas-to-hack/ still updated with useful snippets of info 5 years later.

The Cranky Sysadmin showed how easy it was to get started on this, and sold me my first G1 ! http://blog.2gn.com/category/pano-logic/

Cyrozap has been very helpful and encouraging and provided the first full Pano G2 .ucf file I found https://github.com/cyrozap/Pano-Logic-Zero-Client-G2-FPGA-Demo

Tom Verbeure is doing some interesting work with SpinalHDL and Scala. https://github.com/tomverbeure/panologic-g2

This is an interesting paper http://www.fabienm.eu/flf/wp-content/uploads/2014/11/Note2008.pdf, I made a copy of the G2 bitstream, and spent quite a bit of time trying their methodology and using their software http://florianbenz.github.io/bil/index.html, but ultimately came to the conclusion it would need far too much work to generate a finished product. I'm really interested in what the software architecture of the Pano G2 firware is - is it all native FPGA code (VHDL, Verilog, whatever) or have they just built a big *PC* using a soft processor (MicroBlaze or whatever) and writted the software in C? Maybe one day we'll find out.

G1 schematics that were published on Hackaday by JVisitor - [here](..files/g1_schematics.zip)

Pano the company may be dead, but the help blog lives on: http://panologichelp.blogspot.co.uk/, one or two snippets in there that might be interesting, and some possibly useful disassembly targets if any one is interested, eg. http://panologichelp.blogspot.co.uk/2013/07/how-to-upgrade-xilinx-spartan-6-fpga.html

One of the major drawbacks with the G2, is the Marvell 88E1119 ethernet phy. Marvell are totally hostile to the hacking community, and this part does not have an available datasheet, inspite of it being, what, 7/8 years old now. The closest available seems to be the 88E1111. The other issue is that Xilinx software cores are tightly licenced, and big bucks. All this means is that someone will have to cobble together a driver for a complex part with no datasheet! Something of a challenge. Anyway, two references that I have found that might be of some interest: 
* Philipp Kerling implemented an ethernet MAC in VHDL for a university project http://katalog.bibliothek.tu-ilmenau.de/DB=1/PPN?PPN=834804387 one of the plus points for this is since it is a uni project, it is well documented.
* Joel has a Verilog UDP implementation that may be useful (albeit for an 88E1111) https://joelw.id.au/FPGA/DigilentAtlysResources 
