# SH101 MIDI IO
PCB assembly for TRS-DIN MIDI connections to SH-101

![pcb assembly](/orthoview.jpeg)

## Overview
[Tubbutec](https://tubbutec.de/sh-1oh1/) make an amazing upgrade kit for the Roland SH-101 that replaces the original CPU, adds MIDI, some new modulation sources, and an enhanced sequencer and arpeggiator. The kit comes with a pair of MIDI jacks that can be mounted by drilling holes in the enclosure, or concealed in the battery compartment. This respository contains the design files to build a TRS adapter board to replace the SH-101's MODULATION GRIP PCB, which allows the use of Type A TRS-MIDI cables. The MIDI IN uses the 3.5 MM jack and the MIDI OUT uses the 2.5 MM jack. To get the jacks to the right height, a PCB sandwich is required with 1.5 MM spacers. I used SMT M3 spacers, but a regular PCB spacer of the right height should work as well. There's enough room in the enclsoure to leave the original MODULATION GRIP PCB, so it does not need to be disconnected or removed. The jack PCB needs to be 1 MM thick, and the spacer PCB needs to be 1.6 MM thick.

The project was designed in Kicad 6.0. The BOM and pos files for PCBA of the modulation grip replacement board with SMT spacers have been formatted for the JLC PCBA service.

## BOM

| Part Ref | Description | Part No |
| -------- | ----------- | ------- |
| J1 | 3.5 MM JACK | CUI SJ1-3523N |
| J2 | 2.5 MM JACK | CUI SJ1-2503A |
| J3 | 5 POS HEADER | 0.100" RIGHT ANGLE |
| SM1-4 | 1.5 MM SPACER | SMTSO3015CTJ |

You'll also need a Type A 3.5 MM TRS MIDI cable and a 2.5 MM TRS MIDI cable if you want access to MIDI OUT data. The 2.5 MM TRS to MIDI cable isn't as widely availabe, but is used by a lot of IK Multimedia iRig series products.

## PCBs

The PCB fabrication files are in the [gerbers](/gerbers/) folder. _SH101_IO.zip_ contains the gerber files for the 1 MM thick jack board and _SH101_MOD_GRIP_BOARD.zip_ contains the gerbers for the 1.6 MM modulation grip replacement board. 

## Assembly

![pcb guts](/sh-101-mod-guts-pcb.jpg)




