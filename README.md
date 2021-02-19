# open_robot_dagor_hardware

Robot hardware design from the Open Robot Dynamic Initiative remixed for easier and cheaper assembly using commonly available FDM 3D printers and control via the Dagor brushless motor controller.

This work is based on the [Open Robot Dynamic Initiative](https://github.com/open-dynamic-robot-initiative/open_robot_actuator_hardware) designs. More documentation is following soon.

## Bill of Materials

TBD


## Printing the parts

All the parts pictured in this repository were printed on an Ender 3 FDM printer using various PLA materials. The recommended layer height for printing is 0.2mm, but it should be possible to adjust this.

### Tolerances

The parts are modelled exact without taking into account deviations in hole sizing when 3D printing. This means a hole that is supposed to have a 5mm diameter is modelled exactly as 5mm. To adjust for your printer and filament, it is recommended to print the center transmission pulley (the one with both a 10 tooth and 30 tooth part), and press-fit an MR105 bearing into the shaft on the top and the hole on the bottom of the pulley. The fit should be snug and not have any wiggle to it, but the top bearing should also come off without breaking the part.

To adjust tolerances on an FDM printer use the "XY Size Compensation" in PrusaSlicer or the "Hole Horizontal Expansion" setting in Ultimaker Cura. Try adjusting them in 0.1mm steps for the best fit on the pulley. After this all the other parts should have snug fit as well and work together the best. Keep in mind different filament might need different settings.


## Non-printable parts

There was an attempt to 3D print the ball bearings and belts of the robot, but all of the experiments proved inconclusive. While it is possible to print bearings using a resin 3D printer and belts using flexible filament, both solutions work for prototyping but not the actual working robot due to bad performance.