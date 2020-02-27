# voltmeterMAX1499
The voltmeterMAX1499 is - as you may expect by the name - a voltmeter based on the MAX1499 chip by maximinterated.

Started as a university project (v1) to be put into the student laboratories consoles as a highly accurat voltmeter (guess what: it never happend), it later got reworked (v2) to be used with a refrence voltage and two different seven-segment-display-boards.


## 1 precepts
1. boards for the IC and the 'display' have to be seperate
2. board dimensions not given, but as small as possible
3. six seven-segments – one for the '-' and five for the digits
4. multiple options for displaying (0kR for selection)
	1. decimals by chip
	2. decimals by user
5. boards to be connected by male and female headers
6. drills for spacers and mounting
7. use smd parts


## 2 prototype pictures
![ ](https://github.com/derwana/voltmeterMAX1499/blob/master/pictures/v1_iso.jpg  "prototype v1")
![ ](https://github.com/derwana/voltmeterMAX1499/blob/master/pictures/v1_front.jpg  "prototype v1 front")
![ ](https://github.com/derwana/voltmeterMAX1499/blob/master/pictures/v1_back.jpg  "prototype v1 back")


## 3 prototype testing
on X3: 5V DC (Vcc)
on X1: 1.000V DC (testvoltage by signalgenerator)

Measuring the current consumption is a good tool to determin a correctly working board.

One seven-segment-element consumes 20mA on max brightness and all tiles lit. Six of them are used, so a current consumption of ca. 120mA is expected.

With R3=24kR and displaying 18882, the current flowing is 117mA.
On idle, current consumption as expected of the datasheet.


## 4 Costs
estimated 45,00 € (per unit)
* PCBs 16.65€
* MAX1499 13.10€
* 7-Segments 1.00€-2.00€ (per segment-unit)


## 5 version 2 pictures
Connections:
* potentiometer for dimming (black/pink)
* Vcc (black/red)
* voltage to measure (black/orange)
* programming interface (brown/red/orange/yellow)

![ ](https://github.com/derwana/voltmeterMAX1499/blob/master/pictures/v2_iso.jpg  "prototype v2")
![ ](https://github.com/derwana/voltmeterMAX1499/blob/master/pictures/v2_back.jpg  "prototype v2 back")

## 6 further possible improvements (by programming)
* moving decimal point
* using internal reference of MAX1499
* reading measurements over serial
