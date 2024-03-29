# The Big One

![image0 (6)](https://github.com/TheZ0/The-Big-One/assets/142558812/33357cc0-8e7c-4cac-852c-9c4e36e9c266)


3D printed 3-stage 1kJ bolt-action projectile accelerator. My most ambitious project thus far, one year start to finish, three interconnected PCBs and over 3kg of PLA filament. 

## Safety Notice
Please do not attempt to build what is shown in this repository or similar unless you have experience working with high voltage (>50V) systems. The voltages used within this device are lethal.
## Performance
* Peak exit velocity (All capacitors charged to 385V) - 61 km/h
* Peak exit energy (100g projectile) - 13.9 J
* Efficiency - 1.4%

## Hardware Details
### Capacitor Charger
Capacitors were charged using a ZVS circuit driving a homemade step-up transformer (see below) to increase the 30VAC across the resonant capacitors of the ZVS up to 550VAC to be used to charge the high voltage capacitors. 

<img src="https://github.com/TheZ0/The-Big-One/assets/142558812/5bb98cbe-304d-47cf-9782-3a394f745221" width="450" height="600">
<img src="https://github.com/TheZ0/The-Big-One/assets/142558812/faace633-92bd-4457-8ac8-14c990e99ffc" width="450" height="600">

### Control Board
The control board was mounted in the middle section. It uses an STM32F401RBT6 to control the timing of the three acceleration stages as well as measures the capacitor bank voltage. Four schottky diodes are also on the board to rectify the transformer output.

![image0 (10)](https://github.com/TheZ0/The-Big-One/assets/142558812/82379ab2-0438-47d0-a273-a6d846258432)