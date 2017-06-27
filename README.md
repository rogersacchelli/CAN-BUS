# CAN BUS

## How it works

A single car can have multiple buses, all of them work on the following principle:

* Two wires inputing:
	* Can High Signal (CANH) +1V over 2.5V
	* Can Low Signal (CANL) -1V over 2.5V
	
Every signal is applied as differential. This method improves the environment to an error free transmission. If signals are not simetrical, then is regarded as noise.
```
           +---+   +-------+   +----+  +--+
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
CANH +-----+   +---+       +---+    +--+  +-------+
2.5v   +------------------------------------------+
CANL +-----+   +---+       +---+    +--+  +-------+
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
           |   |   |       |   |    |  |  |
           +---+   +-------+   +----+  +--+
```

Each bus can also work at different speeds:

* High Speed CAN - 500 Kbit/s to 1 Mbit/sec, depending on cable length.
	* Usually carrying important data as speed, breaking and steering.
* Low Speed CAN - 40 Kbit/s to 125 Kbits/sec.
	* Carries non-sensitive data as A/C temperature, windows, locks.

### Where you find the buses

As we mentioned before, can buses operator 1V above/below 2.5V. It meas that if you find two wires running on 2.5V you centainly found a bus.

### ISO 11898:2003 - Standard and Extended CAN
The ISO 11898 architecture defines the lowest two layers of the seven
layer OSI/ISO model as the data-link layer and physical layer.

#### Standard CAN

![Standard CAN](https://image.ibb.co/cLKrA5/Screenshot_from_2017_06_27_00_00_05.png) 


#### Extended CAN

![Extended CAN](https://preview.ibb.co/iO7NHk/Screenshot_from_2017_06_27_00_02_22.png)

### Connector

OBD-II Connector

![OBD-II Connector](http://www.obdii.com/images/connectorblue.GIF) 

|Pin #|Description|
|---|----|
1| LS-CAN High
2|
3| MS-CAN High
4|Chassis Ground
5|Signal Ground
6|CANH
8| LS-CAN Low
14|CANL
16|Battery +12Vc
