# ChameleonButton64
gonchuki's ChameleonButton updated for tB/x64/WDL

![image](https://github.com/user-attachments/assets/43873440-cde4-4ad3-8381-7552cc2c358d)

Original project: https://github.com/Planet-Source-Code/malachi-chameleon-button-an-awesome-multi-style-button__1-28761


This control worked perfectly in twinBASIC 32bit with 0 modification (apart from AccessKeys not yet being implemented, but that's rarely used and doesn't impact appearance). It took 5 minutes to convert to 64bit: I moved its existing APIs into a conditional compilation block so they'd be active in VB6 but not tB (keeps the same code compatible with both), added WinDevLib, replaced 2 enum values it had custom names for with the official ones, uncommented a custom constant it used that was a combination of real flags for DrawText, then the 64bit upgrade: 5 variables had to be changed from Long to LongPtr. And that did it-- it now works perfectly in 64bit. 
