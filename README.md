# imax-B6-duino
arduino based firmware for the imax b6 charger
THE GOAL IS TO MAKE A SIMPLE ARDUINO SKETCH ... not a unviversal charger software. 
(there is allready a geat project called cheally charger that can do everything.)

- understand how the hardware works (the smps is very interestic to me)
- only one type of battery is supported
- the code shold be as simple as possible
- the charging must start imedialtly after power up or connect the battery

HARDWARE
--------
the imax b6 is a atmega32a based battery charger.
- smps buck boost converter , controlled fully by the arduino
- 6 channel balancer
- current / voltage meters
- 2x16 lcd display and 4 buttons


SETUP ARDUINO
-------------
enable ATMEGA32a compiling
- https://learn.adafruit.com/add-boards-arduino-v164/setup
- add this url in arduino GUI file=>preferences=>BootManager URL : https://mcudude.github.io/MightyCore/package_MCUdude_MightyCore_index.json


USBASP programmer
- (currently iuse a old version of avrdude.exe 14.03.2009 and avrdude.conf from 14.03.2009 ... that allowes using the china usbasp) i must check if the new versions of avrdude works too. i also ordered a USBtinyISP ...  
- nice picture on how connect the wires https://habrastorage.org/files/cc9/dd7/52a/cc9dd752aae141a496b4fbd79da0961f.jpg
 
- USE CTRL-SHIFT-U to upload the codes ... the UPLOAD BUTTON WILL NOT WORK !!!

