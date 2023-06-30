# Quattro-Gelato
 A sweet AWD H-Bot

 ![Small Image of Quattro Gelato](https://github.com/CroXY3D/Quattro-Gelato/blob/main/Images/QG_Small.png)

Quattro Gelato is a fully enclosed AWD 150x300x300 H-BOT printer using The Ice Cream Factory's  Ice Cream Sandwich build technique.

Ice Cream Sandwiches are parts made of laser cut aluminum (typically 2-3mm) sandwiching a central printed plastic core.  This is similar in construction to ACM panels such as DiBond which have an incredible strength to weight ration.  Nearly all load is carried by the much stiffer aluminum panels (75x as stiff as plastic).  The plastic core is merely to space the panels apart.   Additionally for high load situations aluminum spacers also separate the plates.  It should be possible to have the panels made by PCB houses using 2mm aluminum PCBs for about 20% the cost of laser cutting, making the construction technique very inexpensive

This stiffness allows the design to be an H-Bot vs the more common CoreXY fixed XY motor design without the inherent gantry torque on X moves being an issue.  H-Bot has a number of advantages - a single shorter belt path, single belt allows using wider belts.  In this case 15mm 3mm pitch GT3 belting from Gates US.  3mm GT3 also has a curvelinear profile, which allows for better belt-pulley tooth meshing and should minimize ripple in prints that is endemic to belted 3D Printers.

With a build volume of 150x300x300, Quattro Gelato has a very short cross gantry, which is further stiffened by being constructed out of 2mm wall 25mm square aluminum tube.   This tube has 2.2 times the stiffness as a 2020 extrusion while being the same mass.  The Y axis is longer because extending Y doesn't have the same penalty in terms of print quality and it's common to print things long and narrow.  Less common for things to be both long and wide.   300mm of Z (easily extended or reduced) is sufficient for 99%+ of the prints I have ever made.
. 
Toolhead movement is provided by four 2504 or 2804 Nema17 stepper motors.  This doubles the positioning torque and hence accuracy and precision are improved for better layer stacking.  High acceleration and speed are provided by (optional) 48V TMC5160 drives.

The toolhead is all metal except for the part cooling fan duct.  Extruder is the water cooled VzBot Hextrudort CNC paired with a VzBot Goliath Hot End.  The hot end should be able to keep up with the motion system and melt plastic up to ~100mm^3/s (about 8x a V6).  The toolhead center of mass is balanced such that it is nearly centered upon the MGN9 rail.  This will largely eliminate any torsional forces which is a significant source of ringing.  Additionally the MGN9 rail is positioned on the front of the gantry tube, where it provides approximately 3x more stiffness in the Y axis than if it were placed on top of the gantry.

The bed is 8 or 10mm cast aluminum lifted via 9mm 2GT belts by three 5:1 belt reduced drives.  It features proper Maxwell kinematic joints to allow for bed expansion while constraining other motion and to allow automatic bed leveling.   Bed levelling and mesh probing is done with the very precise Euclid probe.  If bed drop happens on motor power off, constant force springs will be added in the same style as CroXY.

Quattro Gelato is fully enclosed with panels on all sides.  There is room for insulation as well.  It uses the so suave rounded type R. 

