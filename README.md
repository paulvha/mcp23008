# mcp23008

This repository contains information + a sample program written in C to connect an MCP23008, 8-bit I/O expander I2c interface, to the Raspberry Pi, using the BCM2835 library.

BCM2835 library
Install latest from BCM2835 from : http://www.airspayce.com/mikem/bcm2835/

1. wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.50.tar.gz
2. tar -zxf bcm2835-1.50.tar.gz		// 1.50 was version number at the time of writting
3. cd bcm2835-1.50
4. ./configure
5. sudo make check
6. sudo make install

Install the MCP23008 sample program
1. cd /home/pi
2. tar -xzvf mcp23008.tar.gz
3. cd  mcp23008

Copy the latest BCM2835.h to MCP23008:
1. cd /home/pi
2. cp bcm2835*/src/bcm2835.h  mcp23008

To compile : ./mc
Make sure you are root and then you should be able to run ./MCP23008.
