# PCB for the Adafruit 128x64 I2C/SPI 1.3" OLED breakout board

<a href="http://www.adafruit.com/products/938"><img src="assets/938.jpg?raw=true" width="500px"><br/>
<a href="http://www.adafruit.com/products/938"><img src="assets/image.jpg?raw=true" width="500px"><br/>
  Click here to purchase one from the Adafruit shop</a>

__Format is EagleCAD schematic and board layout__

These displays are small, only about 1.3" diagonal, but very readable due to the high contrast of an OLED display. This display is made of 128x64 individual white OLED pixels, each one is turned on or off by the controller chip. Because the display makes its own light, no backlight is required. This reduces the power required to run the OLED and is why the display has such high contrast; we really like this miniature display for its crispness!

The driver chip, SSD1306 can communicate in two ways: I2C or SPI. The OLED itself require a 3.3V power supply and 3.3V logic levels for communication, but we include a 3.3V regulator and all pins are fully level shifted so you can use with 5V devices!

We've updated the design to add auto-reset circuitry so that the reset pin is optional. The default interface is now I2C not SPI - since it speaks I2C you can easily connect it up with just two wires (plus power and ground!).  We've even included SparkFun qwiic compatible STEMMA QT connectors for the I2C bus so you don't even need to solder! 

The power requirements depend a little on how much of the display is lit but on average the display uses about 40mA from the 3.3V supply. Built into the OLED driver is a simple switch-cap charge pump that turns 3.3v-5v into a high voltage drive for the OLEDs.

[We have a detailed tutorial and example code in the form of an Arduino library](http://learn.adafruit.com/monochrome-oled-breakouts) for text and graphics. You'll need a microcontroller with more than 1K of RAM since the display must be buffered. The library can print text, bitmaps, pixels, rectangles, circles and lines. It uses 1K of RAM since it needs to buffer the entire display but its very fast! The code is simple to adapt to any other microcontroller.

## License
Adafruit invests time and resources providing this open source design,
please support Adafruit and open-source hardware by purchasing
products from Adafruit!

Designed by Adafruit Industries.
Creative Commons Attribution, Share-Alike license, check license.txt for more information
All text above must be included in any redistribution
