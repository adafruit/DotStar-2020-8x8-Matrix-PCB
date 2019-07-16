## Adafruit DotStar High Density 8x8 Grid - 64 RGB LED Pixel Matrix PCB

<a href="http://www.adafruit.com/products/3444"><img src="assets/3444.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit DotStar High Density 8x8 Grid - 64 RGB LED Pixel Matrix. Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/3444

### Description

Do not eat this LED grid just because it is so colorful and bite-sized! This is the tiniest little LED grid we could make, with 64 full RGB color pixels in a square that is only 1" by 1" square (thats 25.4mm x 25.4mm for you metric-lovers). Best of all, these are little DotStar LEDs, with built in PWM drivers, so you only need two digital I/O pins to get a-glowin'.

But do not be fooled by their small size, each LED is still incredibly, blindingly bright just like the DotStars/NeoPixels you know and love. These are the same integrated LEDs that are used in [our new fancy DotStar strips](https://www.adafruit.com/categories/885) just really small.

Arranged in an 8x8 matrix, each pixel is individually addressable: like NeoPixels, DotStar LEDs have an embedded microcontroller **inside the LED**. You can set the color/brightness of each LED to 24-bit color (8 bits each red green and blue). Each LED acts like a shift register, reading incoming color data on the input pins, and then shifting the previous color data out on the output pin. By sending a long string of data, you can control an 'infinite' number of LEDs. The PWM is built into each LED-chip so once you set the color you can stop talking to the disk and it will continue to PWM all the LEDs for you.

Wiring it up is easy: there are two 4-pad connection ports on the back. Solder wires to the input port (+5V GND ClockIn and DataIn) and provide 5VDC to the +5V and ground pins, then connect the CIN/DIN pin to your microcontroller. If you have hardware SPI, use the SCK and MOSI pins respectively. You'll also need to make a common ground from the 5V power supply to the microcontroller/Arduino. Since each LED can draw as much as 40mA (thats up to 2.5 Amps per panel if all LEDs are on bright white!) we suggest our 5V 2A power supply if you're going to use full brightness and a lot of white. For most uses, you'll see about 0.5A of current per panel, and you can set the brightness to drop that down. Note that so much current through a small board can make it toasty!

To keep the board small, we did not put any small surface-mount capacitors on the front. Instead, there's a power/ground pad set on the back and a 220uF capacitor that you can solder onto the back for a compact fit. There's also four mounting holes that you can use for attachment, or snap them off with pliers if you want a perfect 1" square.

[Check out our tutorial showing wiring, power usage calculations, example code for usage, etc!](https://learn.adafruit.com/adafruit-dotstar-leds)

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional details.
