# open_robot_dagor_hardware

Robot hardware design from the Open Robot Dynamic Initiative remixed for easier and cheaper assembly using commonly available FDM 3D printers and control via the Dagor brushless motor controller.

This work is based on the [Open Robot Dynamic Initiative](https://github.com/open-dynamic-robot-initiative/open_robot_actuator_hardware) designs. The following modifications were made:

  - The body and cover of the actuator modules are modified to make them print easily without supports on an entry level FDM printer in PLA.
  - Change of belt to 3M HTD profile. This curved belt profile might not be ideal in terms of backlash and other performance characteristics, but it is more affordable than the AT3 GENIII Conti belts used in the original ODRI work. Other (trapezoidal) tooth profiles might be better suited for this application.
  - Change of gear ratio from 1:9 to 1:8. This leads to slightly less torque but also faster speed. The change was made to accomodate a bigger transmission pulley with 12/32 instead of 10/30 teeth, which allows printing the pulley on an FDM printer in PLA.
  - Change to 4004 360kV budget motors. Change to mounting holes and design of custom Hex-based motor pulley to avoid having to make a custom motor shaft.
  - Mounting holes to control joints via [Dagor Brushless Controller module](https://www.dagor.dev). 
