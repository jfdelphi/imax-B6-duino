# imax-B6-duino

arduino based firmware for the imax b6 charger
the code is made very simple and can be modied to your needs

HARDWARE
--------
https://ae01.alicdn.com/kf/HTB1x3xjIXXXXXcNXXXXq6xXFXXX1/Free-shipping-IMAX-B6-80W-Digital-RC-Lipo-NiMh-Battery-Balance-Charger-AC-POWER-12V-5A.jpg

the imax b6 is a atmega32a based battery charger.
- smps buck boost converter , controlled fully by the arduino
- 6 channel balancer
- current / voltage meters
- 2x16 lcd display and 4 buttons

CPU
http://www.atmel.com/Images/Atmel-8155-8-bit-Microcontroller-AVR-ATmega32A_Datasheet.pdf
MightyCore PIN ASSIGNMENT
https://camo.githubusercontent.com/8466c1b4ca97bf242f00e61a5dbb8e0b0ff6416d/687474703a2f2f692e696d6775722e636f6d2f5464304e6875672e6a7067

SCHEMATICS
http://ru-radio-electr.livejournal.com/1295897.html
https://static.rcgroups.net/forums/attachments/6/4/9/2/6/3/a8738175-193-1469e1%20IMAX%20SkyRC%20Schematic.jpg?d=1456339330


SETUP ARDUINO dev enviroment
-------------
enable ATMEGA32a compiling
- https://learn.adafruit.com/add-boards-arduino-v164/setup
- add this url in arduino GUI file=>preferences=>BootManager URL : https://mcudude.github.io/MightyCore/package_MCUdude_MightyCore_index.json


USBASP programmer
- (currently iuse a old version of avrdude.exe 14.03.2009 and avrdude.conf from 14.03.2009 ... that allowes using the china usbasp) i must check if the new versions of avrdude works too. i also ordered a USBtinyISP ...  
- nice picture on how connect the wires https://habrastorage.org/files/cc9/dd7/52a/cc9dd752aae141a496b4fbd79da0961f.jpg
 
- USE CTRL-SHIFT-U to upload the codes ... the UPLOAD BUTTON WILL NOT WORK !!!


Current Codes
-------------
THINGS THAT WORK
- lcd display
- buck converter !
  - current limiter
- stage logic
  - the logic to charge lifepo4 batteries
- balancer logic  
- MULTIPLEXER reading the cells voltages
- some basic functions to the buttons

TODO
- boost converter
- boost charger signal ( all cells < 3.5V )
- battery ok signal    ( all cells > 3.0V )
