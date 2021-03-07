# open_robot_dagor_hardware

Robot hardware design from the Open Robot Dynamic Initiative remixed for easier and cheaper assembly using commonly available FDM 3D printers and control via the Dagor brushless motor controller.

This work is based on the [Open Robot Dynamic Initiative](https://github.com/open-dynamic-robot-initiative/open_robot_actuator_hardware) designs. There are a few differences:

  - The body and cover of the actuator modules are modified to make them print easily without supports on an entry level FDM printer in PLA.
  - Change of belt to 3M HTD profile. This curved belt profile might not be ideal in terms of backlash and other performance characteristics, but it is more affordable than the AT3 GENIII Conti belts used in the original ODRI work. Other (trapezoidal) tooth profiles might be better suited for this application.
  - Change to 4004 360kV budget motors. Change to mounting holes and design of custom Hex-based motor pulley to avoid having to make a custom motor shaft.
  - Mounting holes to control joints via Dagor Brushless Controller module. Optional mounting holes for AS5600 based magnetic encoder to control via external board like ...
  - Mounting holes for magnetic encoder on output shaft. This means cable management has to be different.

## Bill of Materials whole robot

### 3D printed parts

| Name 							  | qty | instructions |
| hip_aa_structure_left_side_base		| 1 | tbd |
| hip_aa_structure_left_side_cover	| 1 | tbd |
| hip_aa_structure_right_side_base	| 1 | tbd |
| hip_aa_structure_right_side_cover	| 1 | tbd |
| hip_fe_structure_left_side_base		| 1 | tbd |
| hip_fe_structure_left_side_cover	| 1 | tbd |
| hip_fe_structure_right_side_base	| 1 | tbd |
| hip_fe_structure_right_side_cover	| 1 | tbd |
| upper_leg_structure_base			| 2 | tbd |
| upper_leg_structure_cover			| 2 | tbd |
| lower_leg_structure					| 2 | tbd |
| foot_structure						| 2 | tbd |
| body_structure_biped_back			| 1 | tbd |
| body_structure_biped_bottom			| 1 | tbd |
| body_structure_biped_front			| 1 | tbd |
| body_structure_biped_left_side		| 1 | tbd |
| body_structure_biped_right_side		| 1 | tbd |
| body_structure_top					| 1 | tbd |
| motor_shaft_dagor					| 6 | tbd |
| transmission_pulley					| 6 | tbd |
| output shaft						| 6 | tbd |


## Printing the parts

All the parts pictured in this repository were printed on an Ender 3 FDM printer using various PLA materials. The recommended layer height for printing is 0.2mm, but it should be possible to adjust this.

### Tolerances

The parts are modelled exact without taking into account deviations in hole sizing when 3D printing. This means a hole that is supposed to have a 5mm diameter is modelled exactly as 5mm. To adjust for your printer and filament, it is recommended to print the center transmission pulley (the one with both a 10 tooth and 30 tooth part), and press-fit an MR105 bearing into the shaft on the top and the hole on the bottom of the pulley. The fit should be snug and not have any wiggle to it, but the top bearing should also come off without breaking the part.

To adjust tolerances on an FDM printer use the "XY Size Compensation" in PrusaSlicer or the "Hole Horizontal Expansion" setting in Ultimaker Cura. Try adjusting them in 0.1mm steps for the best fit on the pulley. After this all the other parts should have snug fit as well and work together the best. Keep in mind different filament might need different settings.


## Non-printable parts

There was an attempt to 3D print the ball bearings and belts of the robot, but all of the experiments proved inconclusive. While it is possible to print bearings using a resin 3D printer and belts using flexible filament, both solutions work for prototyping but not the actual working robot due to bad performance.