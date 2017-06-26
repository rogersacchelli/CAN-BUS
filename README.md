# CAN BUS

## How it works

* Two wires
	* Can High (CANH) +1V
	* Can Low (CANL) 	-1V
	
Every signal is applied as a positive signal at CANH wire and as the oposite value to CANL. This method improves the environment to an error free transmission. If signals are not simetrical, then is regarded as noise.
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

### Connector

OBD-II Connector

![OBD-II Connector](http://www.obdii.com/images/connectorblue.GIF) 

|Pin #|Description|
|---|----|
1|
2|
3
6|CANH
14|CANL
16|Battery +12Vc
