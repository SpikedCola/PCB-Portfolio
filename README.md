# PCB Portfolio

These are some PCBs I have laid out over the last couple years. 

Older boards were designed with DIY-etching in mind (text in the copper layer, fewer vias, etc.). Newer boards were made through [OSHPark](http://www.oshpark.com/) and were designed to pass their DRC.

If you are interested in discussing one of my designs, or would like to hire me, please contact me [through email](mailto:parkinglotlust@gmail.com).

Cheers,
<br />
- Jordan

## Xbox NAND Flasher
This board went through several design iterations. It started out as a way to flash the SPI NAND chip on an Xbox360. Eventually a [group-buy](https://web.archive.org/web/20120404002711/http://forums.xbox-scene.com/index.php?showtopic=699595) for these devices was started, and I producing and assembled a panel of these boards. Lesson learned: pay someone else to fab boards! DIY boards should *not* be sold en-masse.

Two revisions are shown; the newer of the two shows the addition of an integrated USB-B connector, extra features (ability to output serial, built-in bootloader for reflashing), and bug-fixes (a crystal turned out to be much more stable than a resonator).

### v2.0 Schematic
[![v2.0 Schematic](xbox-nand-flasher/thumbs/v2.0-schematic.png)](xbox-nand-flasher/v2.0-schematic.png)
### v2.0 Board
[![v2.0 Board](xbox-nand-flasher/thumbs/v2.0-board.png)](xbox-nand-flasher/v2.0-board.png)
### v2.3 Schematic
[![v2.3 Schematic](xbox-nand-flasher/thumbs/v2.3-schematic.png)](xbox-nand-flasher/v2.3-schematic.png)
### v2.3 Board
[![v2.3 Board](xbox-nand-flasher/thumbs/v2.3-board.png)](xbox-nand-flasher/v2.3-board.png)

Beat Detector
-------------
This board uses a low-pass filter, envelope detector and a comparator to flash lights to the beat of music. It also has a power MOSFET to drive a decent-sized load (I was driving about 50 LEDs).

If I made another version of this board, I would likely drop the monostable 555 as I'm not really a fan of it's effect. Or possibly add a bypass switch, or more adjustments. Would also rework it to be much smaller, and with more convenient mounting holes.

### Schematic
[![Schematic](beat-detector/thumbs/schematic.png)](beat-detector/schematic.png)
### Board
[![Board](beat-detector/thumbs/board.png)](beat-detector/board.png)

LiPo Power Supply
-----------------

Unfortunately I've lost the schematic for this one... 

The board uses a MAX1555 to provide charging functionality for a LiPo battery. Power is provided via a mini-B USB port, or a DC barrel jack. 

A boost regulator is used to step the 3.7v output voltage up to 5v. An LDO was used to provide a clean 3.3v signal for an accelerometer and gyro.

### Board
[![Board](lipo-power-supply/thumbs/board.png)](lipo-power-supply/board.png)

Breadboard Power Supply
-----------------------

This project turned out to be very helpful when working with op-amps. The board is sized to plug directly into a breadboard, and the inductors on the back keep the board at the correct height off the desk/table. 

Adjustment switches and knobs allow the output voltage to be preset, or adjusted.

### Schematic
[![Schematic](breadboard-power-supply/thumbs/schematic.png)](breadboard-power-supply/schematic.png)
### Board
[![Board](breadboard-power-supply/thumbs/board.png)](breadboard-power-supply/board.png)

Lift Light
----------
This was a small board I created for a car I owned (A 7th-gen Toyota Celica). I wanted a light to turn on when the engine's "Lift" (VVTL-I) was activated. 

When "Lift" was activated, a 10% 200Hz square wave signal would go to 100% duty. To detect this condition, a simple 2.5Hz LPF is used to filter out the 200Hz signal. The output is fed to an op-amp, which drives a MOSFET (and eventually a load). 

The circuit board was designed to be small enough to fit in-line and be covered with heatshrink tubing.

### Schematic
[![Schematic](lift-light/thumbs/schematic.png)](lift-light/schematic.png)
### Board Top
[![Board](lift-light/thumbs/board-top.png)](lift-light/board-top.png)
### Board Bottom
[![Board](lift-light/thumbs/board-bottom.png)](lift-light/board-bottom.png)

Aircraft Receiver
-----------------

This project is still a Work-In-Progress and the final design is un-tested.

The design of this circuit comes from [this site for an Aviation Band Receiver](http://www.sentex.ca/~mec1995/circ/aviarx/aviarx.html), with the board designed to fit perfectly inside [this Hammond enclosure](http://www.hammondmfg.com/pdf/1593L.pdf).

### Schematic
[![Schematic](aircraft-receiver/thumbs/schematic.png)](aircraft-receiver/schematic.png)
### Board Top
[![Board](aircraft-receiver/thumbs/board-top.png)](aircraft-receiver/board-top.png)
### Board Bottom
[![Board](aircraft-receiver/thumbs/board-bottom.png)](aircraft-receiver/board-bottom.png)
