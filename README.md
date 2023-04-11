# MCU-3DL (MicroController Unit for 3D Location)

The goal of this project is to design manufacture and program a board with collection of all the data about the 3D location of the board and a system to strore and send live this data to any devices.


## Design

This board will be composed of 3 processing unit, one for the processing of the measurements, one for handeling with the comunication and the main processing unit

### MPU (Main Processing Unit) 
The main controller for this board will be a STM32F412CGU6. It will probably be way overkill for any task it will be assigned to, but we never know.

### NPU (Navigation Processing Unit)
This controller will be a STM8AF5286UAY. It take the measurements of all the sensors and will do all the filters and sensor fusion calculation.

### TPU (Telemetry Processing Unit)
This controller will be a STM8AF5286UAY. It will store the position data into the SD card and will communicate them via Bluetooth or radio.

### Sensors
The sensors chosen for this project are :
- #### Gyroscope and Accelerometer : LSM6DSRXTR
- #### Magnetometer : IIS2MDCTR
- #### Barometer: LPS22DFTR
- 


ATSAMD21
UBLOX ZOE M8Q
NRF8001

