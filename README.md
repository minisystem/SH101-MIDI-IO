# SH101 MIDI IO
PCB assembly for TRS-DIN MIDI connections to SH-101

![pcb assembly](/views.png)

## Overview
[Tubbutec](https://tubbutec.de/sh-1oh1/) make an amazing upgrade kit for the Roland SH-101 that replaces the original CPU, adding MIDI, some new modulation sources, and an enhanced sequencer and arpeggiator. The kit comes with a pair of MIDI jacks that can be mounted by drilling holes in the enclosure, or concealed in the battery compartment. This respository contains the design files to build a TRS adapter board to replace the SH-101's MODULATION GRIP PCB, which allows the use of Type A TRS-MIDI cables. The MIDI IN uses the 3.5 MM jack and the MIDI OUT uses the 2.5 MM jack. To get the jacks to the right height, a PCB sandwich is required with 1.5 MM spacers. I used SMT M3 spacers, but a regular PCB spacer of the right height should work as well. There's enough room in the enclsoure to leave the original MODULATION GRIP PCB, so it does not need to be disconnected or removed. The jack PCB needs to be 1 MM thick, and the spacer PCB needs to be 1.6 MM thick.

The project was designed in Kicad 6.0. The BOM and pos files for PCBA of the modulation grip spacer PCB with SMT spacers have been formatted for the JLC PCBA service.

## BOM

| Part Ref | Description | Part No |
| -------- | ----------- | ------- |
| J1 | 3.5 MM JACK | CUI SJ1-3523N |
| J2 | 2.5 MM JACK | CUI SJ1-2503A |
| J3 | 5 POS HEADER | 0.100" RIGHT ANGLE |
| SM1-4 | 1.5 MM M3 SPACER | SMTSO3015CTJ |

You'll also need a Type A 3.5 MM TRS MIDI cable and a 2.5 MM TRS MIDI cable if you want access to MIDI OUT data. The 2.5 MM TRS to MIDI cable isn't as widely availabe, but is used by a lot of IK Multimedia iRig series products.

## PCBs

The PCB fabrication files are in the [gerbers](/gerbers/) folder. _SH101_IO.zip_ contains the gerber files for the 1 MM thick jack board and _SH101_MOD_GRIP_BOARD.zip_ contains the gerbers for the 1.6 MM modulation grip spacer board. 

## Assembly

Once assembled, the PCB sandwich slides into guide slots of the plastic enclosure. Tape the original modulation grip jack board to the side of the enclosure. Use a 5 conductor connector assembly, crimp contacts, 0.100" pitch (TE 5-103975-4 or equivalent). Refer to the schematic and PCB markings for wiring order.

The Type A TRS wiring is as follows:

MIDI 4 (source) > RING

MIDI 2 (shield) > SLEEVE

MIDI 5 (sink) > TIP


![pcb guts](/sh-101-mod-guts-pcb.jpg)




