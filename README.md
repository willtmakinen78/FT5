# FT5
My Very first 3D printer, this is a brief overview of the modifications I've made to my Folgertech FT-5 over the years.

Like the [BCN3D Sigma](https://github.com/willtmakinen78/BCN3DSigma), my work on this machine has been somewhat haphazard and disjointed, so I've done mmy best to collect the most recent version of things here. As my very first machine, this printer has gone through a lot, with many different changes made over the years, both big and small. It was a great learning platform, as it is quite large (300mmx300mmx500mm build volume) with a very open frame, and lent itself quite well to be used for my HIgh school Junior year science fair project which you can check out [here](https://github.com/willtmakinen78/sciencefair2017). If you compare the pcitures between the two, you could somewhat track how it's changed over the years.

#### Here is a list of (most) of the changes I've made:
- Replaced extruder with the E3D Hemera
  - perhaps it's because I'm an E3D shill due to my interning with them, but this is a really great extruder. After going through the stock extruder, the E3D Titan Aero, and a Bondtech Extruder, this has proved to be the best one yet, with the most consistently-good print quality.
  - This is also accompanied by a custom layer fan duct due to the non-standard mounting, similar to the ones on my Sigma printer.
  - an entirely new 3d printed extruder mount was also needed.
 - Aluminum bed mount and BuildTak FlexPlate System
  - the aluminum bed mount provides a super flat base surface for the silicone heater (also added) and the FlexPlate allows for induction probing and easy-to-remove prints
- Induction probe for automatic bed leveling
  - given the era of the FT5 and its price, I don't blame Folgertech too much for not including auto med leveling. After running a BLTouch for a number of years, I wanted something that wouldn't get destroyed if the probe was accidentally left out while an illegal move was being made, so the induction probe is a great solution with no moving parts that triggers perfectly well with the metal FlexPlate.
- Larger overhead spool holder
  - Another feature that has gone through many different iterations, this spolholder, of a size that could only be printed on the FT-5 itself, is finally something that I'm really statisfied with. The bowden tube also prevents the spools from unspooling when you let go of the filament, which is a nice feature.
- Unified Z-axis
  - this one was pulled straight from Thingiverse, but it's a nice little touch that ensures the two Z motors are always moving in sync.
- Integrated RaspberryPi with 7in touch screen
  - I love being able to control my printers from the machines themselves, and this giant touchscreen with a pi running Repeteier Host makes that super easy. It also looks really cool.
- ATX power supply
  - the standard PSU died on me, so I went all out and bought an ATX PSU to replace it (it's a 12V printer). It also has RGB.
- Added TMC2130 stepper drivers
  - replaced the default A4988s with the trinamics to allow for super quiet StealthChop operation and SPI/software-controlled motor currents.
- Improved cable management and wiring harness to the extruder
  - replaced the heavy and drag-prone cable chains with a single wire bundle wrapped in a nice braided sleeve.
- Added print light
  - this is ther same light used for the science fair project. It's meant to be mounted to cars as an auxillary headlight so it's super bright and makes it really easy to see what you're doing and illuminates things very well for the webcam connected to Repetier Host.
- Fully custom Marlin configuration
  - done to keep things updated to the most recent version. The default firware was luckily also a pretty stock Marlin, but Folgertech never really sent out too many updates.
- Fully custom PrusaSlicer Settings
  - This machine has printed GCode from almost any slicer imagineable (Slic3r, Cura, Simplify3D), however PrusaSlicer is my current favorite due to how it handles the differences between machines, gneral print settings, and materials.
- Unified white printed parts
  - tool holders, wire clips, etc. The little things.
