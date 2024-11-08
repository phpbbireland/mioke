# Mioke Keyboards
More keyboards for qmk/via [ayla80, ayla100]  

Ayla80: QMK/VIA based Open Hardware Keyboard with 99 Keys (including macro keys)  
Ayla100: QMK/Via full size Keyboard including Macro Keys  

Development is broken into the following steps:  
1) A very basic keyboard PCB (contains the key switches, diodes and RGB, and no micro)...  
2) A Blackpill Module (connected via the usual two 20 pin connectors)...
3) Once development is complete we then combine both in one PCB...

I have also designed a new development board to replace the Blackpill for future development.  
It adds additional GPIO to allow a 6x17 matrix and additional signals for example, Caps Lock etc...  

The new dev board connects via a small 30 pin 1.27mm pitch connector or possibly a ribbon cable, both are being considered.  
There are several advantages to having the main electronics on a separate board but it's primarily to ease development.  

Ref: https://hackaday.io/project/197065-mioke80-iso-99-key-80-keyboard  

+ Keyboard schematic prototype complete...
+ Controller schematic prototype complete...
+ Software 90% complete...  
+ QMK/VIA code tested on Blackpill 411 Dev Board
+ QMK/VIA code not tested on new dev controller board (Blackpill 411 replacement Dev Board with more GPIOs)
+ Blackpilll version now loads in usevia.app... RGB, Encoder and layout stil needs work...

Kicad Resources:  
[https://github.com/ebastler/marbastlib](https://github.com/ebastler/marbastlib)  
[https://github.com/joe-scotto/scottokeebs](https://github.com/joe-scotto/scottokeebs)

Matrix 10X10 (keyboard-layout-editor.com)
```
[{f:5},"0,0",{x:0.25},"0,1",{x:1},"0,2","0,3","0,4","0,5",{x:0.5},"0,6","0,7","0,8","0,9",{x:0.5},"1,0","1,1","1,2","1,3",{x:0.25,f:4},"1,4","1,5","1,6"],
[{y:0.25,f:5},"1,7",{x:0.25},"1,8","1,9","2,0","2,1","2,2","2,3","2,4","2,5","2,6","2,7","2,8","2,9","3,0",{w:2},"3,1",{x:0.25,f:4},"3,2","3,3","3,4"],
[{f:5},"3,5",{x:0.25,w:1.5},"3,6","3,7","3,8","3,9","4,0","4,1","4,2","4,3","4,4","4,5","4,6","4,7","4,8",{x:0.25,a:6,w:1.25,h:2,w2:1.5,h2:1,x2:-0.25},"6,6",{x:0.25,a:4,f:4},"4,9","5,0","5,1"],
[{f:5},"5,2",{x:0.25,w:1.75},"5,3","5,4","5,5","5,6","5,7","5,8","5,9","6,0","6,1","6,2","6,3","6,4","6,5",{x:1.5,f:4},"6,7","6,8","6,9"],
[{f:5},"7,0",{x:0.25,w:1.25},"7,1","7,2","7,3","7,4","7,5","7,6","7,7","7,8","7,9","8,0","8,1","8,2",{w:2.75},"8,3",{x:0.25},"8,4",{f:4},"8,5","8,6"],
[{f:5},"8,7",{x:0.25,w:1.25},"8,8",{w:1.25},"8,9",{w:1.25},"9,0",{w:6.25},"9,1",{w:1.25},"9,2",{w:1.25},"9,3",{w:1.25},"9,4",{w:1.25},"9,5",{x:0.25,f:4},"9,6","9,7","9,8","9,9"]

```

This is a work in progress...
