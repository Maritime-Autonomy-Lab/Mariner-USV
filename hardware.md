## Sensors
We have intergrated the following sensors onboard Mariner. 
- Oculus M750d imaging sonar
- Ouster LiDAR
- VN100 IMU
- Tac-450 FOG
- Here 3+ GPS
- Nortek DVL 1000

## CAD
Each sensor has a custom mount, which attaches it to the 80/20 frame. Each sensor mount is detailed in the Onshape workspace for Mariner. 

Link to onshape: link here

## CAD for internals
Inside the project box mounted on the Mariner USV we have a series of acrylic trays to mount the relavant parts. The intent of this design is not to mount items to the tray, each item gets mounted to a 3D printed bracket, which then gets screwed into the tray. Each tray has holes sized to tap threads for 4-40 standard screws. These trays and mounting plates are all availble in this repo. 
- Link to project box: https://www.digikey.com/en/products/detail/bud-industries/PTR-28495/17765917

## Control and Communications System
We do not use the provided bluerobotics radios. We have three sets of radios for different purposes.
- RFD-900 #1: This radio is for controlling the robot, pushing missions, etc. 
- RFD-900 #2: This radio is for RTK corrections. 
- Rajant 5Ghz: This radio is to ssh into the rasberry pi inside the project box and visualize any data coming back off the boat. 

## Manual Control 
We use an xbox controller for manual control, via Q ground control. Diagram below. 

<img src="images/USV Controller.jpg" width="400">

## Power Distribution
There are many devices onboard the vehicle that require different voltages of power. To deal with this we have a custom PCB that uses Pololu regulators. This will provide 5, 12, 24 and raw battery voltage. Note we use bluerobotics batteries. The Mariner power distrubtion board requires the following parts. We list their names and digikey part numbers. The PCB part file is located here: LINK HERE. 

- Terminal block, 1x, 277-1364-ND
- Terminal block, 4x, 277-1360-ND
- 24 volt regulator, 2x, 2183-2569-ND
- 12 volt regulator, 1x, 2183-4095-ND
- 5 volt regulator, 1x 2183-4091-ND
- Terminal block, 1x, 732-10955-ND
- Header, 1x, 455-B2B-XH-A-ND

## Wiring diagram
Below we provide a diagram that includes all devices inside the project box. 

<img src="images/Wiring Diagram.png" width="400">

