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
