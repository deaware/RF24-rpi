RF24-rpi
========

Fork from [https://github.com/jscrane/RF24-rpi](https://github.com/jscrane/RF24-rpi).
And patch for Raspberry Pi 2.


setup the library
=================

Clone or download this repo then go to folder

```Shell
git clone https://github.com/deaware/RF24-rpi.git
cd RF24-rpi
```

then 

```Shell
make
make install
```


Usage
=====

// Setup for GPIO 22 CE and CE1 CSN with SPI Speed @ 8Mhz
RF24 radio(RPI_V2_GPIO_P1_15, RPI_V2_GPIO_P1_26, BCM2835_SPI_SPEED_8MHZ);  


Wiring
======

```Shell
nRF24L01+                  Raspberry Pi 2

GND          <----->       GND
VCC          <----->       +3.3V
CE           <----->       GPIO22 [15]
CSN          <----->       GPIO7 [26]
SCK          <----->       GPIO11 (SPI_CLK) [23]
MOSI         <----->       GPIO10 (SPI_MOSI) [19]
MISO         <----->       GPIO9 (SPI_MISO) [21]
```
