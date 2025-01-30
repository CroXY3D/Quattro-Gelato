# Quattro-Gelato
 A sweet AWD 3Z Cartesian

 ![Small Image of Quattro Gelato](https://github.com/CroXY3D/Quattro-Gelato/blob/main/Images/QG_Small.png)

Quattro Gelato is a fully enclosed AWD 150x300x300 cartesian printer using The Ice Cream Factory's  Ice Cream Sandwich build technique.

Ice Cream Sandwiches are parts made of laser cut aluminum (typically 2-3mm) sandwiching a central printed plastic core or metal standoffs.  This is similar in construction to ACM panels such as DiBond which have an incredible strength to weight ration.  Nearly all load is carried by the much stiffer aluminum panels (75x as stiff as plastic).  The plastic core is merely to space the panels apart.   Additionally for high load situations aluminum spacers also separate the plates.  It should be possible to have the panels made by PCB houses using 2mm aluminum PCBs for about 20% the cost of laser cutting, making the construction technique very inexpensive

This stiffness allows the design to be a cartesian vs the more common CoreXY fixed XY motor design without the inherent gantry torque on X moves being an issue.  Cartesian has a number of advantages - a much shorter belt paths, single belt allows using wider belts.  In this case 12mm 2mm pitch GT3 belting for Y and 9mm 2GT3 for X.   


With a build volume of 150x300x300, Quattro Gelato has a very short cross gantry to maximize stiffness where single gantry printers are weakest. The Y axis is longer because extending Y doesn't have the same penalty in terms of print quality and it's common to print things long and narrow.  Less common for things to be both long and wide.   300mm of Z (easily extended or reduced) is sufficient for 99%+ of the prints I have ever made. 

 ![Quattro Gelato Motors](https://github.com/CroXY3D/Quattro-Gelato/blob/main/Images/QG_Motors.png)

Toolhead movement is provided by four 2504 Nema17 stepper motors.  This doubles the positioning torque and hence accuracy and precision are improved for better layer stacking.  High acceleration and speed are provided by (optional) 48V TMC5160 drives.

 ![Quattro Gelato Toolhead](https://github.com/CroXY3D/Quattro-Gelato/blob/main/Images/QG_Toolhead.png)
 (This is an old design.  will be updated soon)
 
(OLD) The toolhead is all metal except for the part cooling fan duct.  Extruder is the water cooled VzBot Hextrudort CNC paired with a VzBot Goliath Hot End.  The hot end should be able to keep up with the motion system and melt plastic up to ~100mm^3/s (about 8x a V6).  The toolhead center of mass is balanced such that it is nearly centered upon the MGN9 rail.  This will largely eliminate any torsional forces which is a significant source of ringing.

 ![Quattro Gelato Gantry](https://github.com/CroXY3D/Quattro-Gelato/blob/main/Images/QG_CPAP.png)
 
Part cooling is via CPAP and the design is compatible with the many excellent VZBot cooling ducts available.

The bed is 8 or 10mm cast aluminum lifted via 6mm 2GT belts by three 30:1 harmonic drive  reduced drives.  It features proper Maxwell kinematic joints to allow for bed expansion while constraining other motion and to allow automatic bed leveling.   Bed levelling and mesh probing is done with the very precise Euclid probe.  If bed drop happens on motor power off, constant force springs will be added in the same style as CroXY.

Quattro Gelato is fully enclosed with panels on all sides.  There is room for insulation as well.  It uses the so suave rounded type R. 

