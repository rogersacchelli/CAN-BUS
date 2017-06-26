# CAN BUS

## How it works

* Two wires
	* Can High (CANH)
	* Can Low (CANL)
	
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