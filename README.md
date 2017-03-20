# lcd-16x2-i2c-pcf8574-pi4j
Class helper for integration LCD 16x2 I2C + module PCF8574 with Raspberry PI and pi4j. 

This module usualy use address 0x3f. For check that in your PI with command i2cdetect -y 1.

For connect PCF8574 module to RaspPi you need use level voltage converter:
RPi      |                  | LCD
------------------------------------
VCC 5v   | <------------->  | VCC 5v
SDA 3.3v | <--CONVERTER-->  | SDA 5v
SCL 3.3v | <--CONVERTER-->  | SCL 5v
GND      | <------------->  | GND
