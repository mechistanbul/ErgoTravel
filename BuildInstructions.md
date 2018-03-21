# ErgoTravel Build Instructions

---

## Review your parts

### Electronic Parts List

- [ ] 2 PCBs
- [ ] 2 5V/16MHz Pro Micros
- [ ] 2 Sockets
- [ ] 2 4.7k resistors. Through Hole and SMD supported
- [ ] 2 surface mount TRRS Jacks (PJ-320D-A)
- [ ] 2 surface mount reset switches (switch 5.25.21.5 250gf Copper head)
- [ ] 54 1N4148 Diodes. Through Hole and SMD supported
- [ ] 1 TRRS Cable

### Optional: For RGB Underglow

- [ ] 2 WS2812 Strips

### Option 1: PCB Sandwich Case Parts List

- [ ] 2 Top PCB Plates
- [ ] 2 Bottom PCB Plates
- [ ] 18 M2x4mm screws
- [ ] 9 M2x12mm standoffs


### Option 2: PCB Mount Case Parts List

- [ ] 2 PCBs (same PCBs will be used for Bottom Plates)
- [ ] 12 M2x4mm screws
- [ ] 6 M2x12mm standoffs


### Option 3: 3D Printed Case Parts List (3D Printed Case not available yet)

- [ ] Left Case Top
- [ ] Left Case Bottom
- [ ] Right Case Top
- [ ] Right Case Bottom

### Switches and stabilizers

The number of switches and stabilizers depends on the desired configuration for the thumb switches.

| Configuration | Switches | 2U Cherry Stabilizer |
| :---: | :---: | :---: |
| 4x1U  |  54   |  0  |
| 2x1U + 1x2U  |  53   |  1  |
| 2x2U  |  52   |  2  |


---

## Prepare PCBs and Install Components

### Step 1: Place PCBs face up with thumbs facing inward.

To avoid building two left or two right halfes, place the PCBs side by side with the thumbs facing toward each other.

PLACE IMAGE HERE

### Step 2: Decide which half will be the master.

The Master half will be connected to the USB port.  This will decide where we install the I2C resistors. 
Note: In the end, it doesn't matter much if you have the resistors on the slave.

Divide the components in two halves and keep with each PCBs.
Put the 2 resistors with the master half.

PLACE IMAGE HERE

Note: Unlike some other keyboards, there are no jumpers to configure for the left or right halves.


### Step 3: Install the diodes

Install all diodes on top side.   

Black line on the diode lines up with the square pad and white line on the PCB silkscreen, bend the legs and push it through.
![diodes](/images/diodes.png)
Bands must match the bands on the silkscreen.

Take care that the diodes stay outside the switch footprints. This should be easy since there is lots of room in between switches.

If diodes are on the other side, it should still work finel; however, there is a diode under the pro micro and the presence of the diode may prevent the pro micro to be installed properly.

### Step 4: Install the resistors
If you are working on the Master Half, install the resistors near the top, on the top side.
PLACE IMAGE HERE
If you are working on the slave side, continue to the next step. The slave side does not have resistors.  
If resistors are on installed the slave instead of the master, it should still work fine.


### Step 5: Install Reset Switch

Install Reset switch on the bottom side of the boards. This is a surface mount switch.  Apply some solder to one of the 4 pads. Place the switch in position.  Melt the pre-applied solder to "tack" the switch in place. Solder the other 3 connections.
PLACE IMAGE HERE
Some recommend to put some solder on the 4 pads.  I find it easier to align the switch if only 1 pad has solder pre-applied.  Using tweezers, you can hold the switch and gently touch the leg with the soldering iron and melt the solder. Let the solder solidify and solder the other legs.  

### Step 6: Install TRRS Connector

Install TRRS Connector on the bottom side of the boards. This is a surface mount connector.  Apply some solder to one of the 4 pads; preferably to the side that had a single connection. Place the connector in position.  Melt the pre-applied solder to "tack" the connector in place. Solder the other 3 connections.
PLACE IMAGE HERE
Some recommend to put some solder on the 4 pads.  I find it easier to align the connector if only 1 pad has solder pre-applied.  Using tweezers, you can hold it and gently touch the leg with the soldering iron and melt the solder. Let the solder solidify and solder the other legs.  


### Step 7: Option 1 (recommended) Install Pro Micro Sockets 
Install Pro Micro Sockets on the bottom side of the boards. DO NOT SOLDER THE PRO MICRO.
PLACE IMAGE HERE

### Step 7: Option 2 (not recommended) Install Pro Micro Headers
Install Pro Micro Headers on the bottom side of the boards. DO NOT SOLDER THE PRO MICRO.
PLACE IMAGE HERE

### Step 8: Validate your soldering job and test the diodes...
Validate that the diodes were installed correctly.  Once the switches are installed through the top plate, it will be close to impossible to replace the diodes without unsoldering everything.

---

## Install Switches
**This is the last time you will have access to the diodes and the other components on the top side.  Double check your work before continuing!**

Place the Top plate above the PCB.

---
## Test and Flash Pro Micros

It's easier to replace a faulty Pro Micro if it's not already installed.

---
## Install Pro Micro

still lots to do...