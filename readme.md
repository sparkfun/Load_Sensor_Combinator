SparkFun Load Sensor Combinator
=============================

![SparkFun Load Sensor Combinator](https://cdn.sparkfun.com//assets/parts/1/0/5/1/1/13281-04.jpg)

[*SparkFun Load Sensor Combinator (BOB-13281)*](https://www.sparkfun.com/products/13281)

Repository Contents
-------------------
* **/Hardware** - Eagle design files (.brd, .sch)

Documentation
--------------
* **[Hookup Guide](https://learn.sparkfun.com/tutorials/load-cell-amplifier-hx711-breakout-hookup-guideL)** - Basic hookup guide.
* **[SparkFun Fritzing repo](https://github.com/sparkfun/Fritzing_Parts)** - Fritzing diagrams for SparkFun products.
* **[SparkFun 3D Model repo](https://github.com/sparkfun/3D_Models)** - 3D models of SparkFun products. 

How to Use
----------
![Combinator PCB](https://cdn.sparkfun.com//assets/parts/1/0/5/1/1/13281-01.jpg)

![Combinator PCB in action](https://cdn.sparkfun.com/r/600-600/assets/learn_tutorials/3/8/3/HX711_and_Combinator_board_hook_up_guide-09.jpg)

If you open up an electronic bathroom scale you’ll find a large rats nest of wires. The Load Sensor Combinator was created to combine the 12 wires found in a bathroom scale into the standard 4-wires that wheatstone bridge configuration.

This board also works with four of our individual [load sensors](https://www.sparkfun.com/products/10245). If you aren’t mechanically inclined we recommend purchasing an off-the-shelf bathroom scale and hacking the combinator into it rather than trying to design a base to properly mount four load sensors.

This board works great with our [Load Cell Amplifier](https://www.sparkfun.com/products/13230) breakout board. The five pins on the edge of the combinator line directly up to the five pins on the amplifier.

If your amplifier and supporting electronics are more than a few inches away from the scale an [RJ45 footprint](https://www.sparkfun.com/products/643) is provided. The 4 wheatstone pins (E+/E-/S+/S-) are connected to twisted pairs within a standard cheap ethernet cable. This allows the amplifier board to be placed many feet away from the scale itself.

The combinator board also includes a footprint for the [DS18B20 one wire temperature sensor](https://www.sparkfun.com/products/245). This allows the user to gather the temperature of the scale in case there is a large variance between the scale and the amplifier. These three pins are exposed to the RJ45 connection as well allowing remote temperature readings to be gathered over one twisted pair ethernet cable.

If you plan to use the RJ45 connection you will need to cut and strip the end of the ethernet cable you do not intend to plug into the combinator board. The wires of the exposed ethernet cable connect to the following pins on the combinator board:

* Combinator Pin = Ethernet cable wire color
* E+ = Brown
* E- = Brown white
* NC = Green
* A+ = Blue white
* A- = Blue
* 5V = Green white
* TEMP_DAT = Orange
* GND = Orange white

The NC pin is intentionally left *not connected*. For especially long cables the signals should be shielded against EMI. This is done by using the less common [shielded twisted pair](http://en.wikipedia.org/wiki/Twisted_pair#Cable_shielding) (STP) ethernet cable. The metal foil sheath of the cable creates a telescoping shield by connecting it to ground on the amplifier circuit, not on GND or any other pin on the combinator board.

License Information
-------------------

This product is _**open source**_! 

Please review the LICENSE.md file for license information. 

If you have any questions or concerns on licensing, please contact techsupport@sparkfun.com.

Distributed as-is; no warranty is given.

- Your friends at SparkFun.
