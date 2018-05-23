
r8.3_1284
---------
* Added diode on FTDI connector's 5V in?
* Connected RS485 RE to DE (prevent receiving stuff you're sending)

r10.0_328_1284
--------------
* Added a ATMega 328 in addition to the 1284
  - Changed various pins on the 1284 layout to mesh better with the 328

r10.1_328_1284_ESP
------------------
* Added block to allow for the addition of an ESP8266 4x2-pin module

r10.1_328_1284_RFM69HCW
-----------------------
* Added block to allow for the addition of a RFM69HCW radio
  - Hardware SPI, SS = D15/D10
  - RFMIRQ = D14/D9
  - Added 10uf and 0.1uf caps
* LED controllers needed to move from hardware to software SPI
  - LED_DATA = D12/D7
  - LED_CLK = D13/D8
* The status LED no longer has particularly useful inputs
  - LED_DATA, LED_CLK, and MISO

r10.2_328_1284_RFM69HCW
-----------------------
* Added ground indicator to FTDI connector
* Added labels to indicate correct level converter orientation
* Moved RFM IRQ to D2 for the ATMega328
