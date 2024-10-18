
# Introduction

The OSE Robot PoE Switch allows the user to easily integrate a Rajant ES1, DX2 and Cardinal or other PoE dependant device to their robotics platform. Two versions of the Robot PoE Switch are available, OEM and Spot. The OEM is intended for third party integrations and the Spot is intended to be mounted on a Boston Dynamics Spot.

# Spot version specifications

The OSE Robot PoE Switch (stand alone) allows the user to easily integrate a Rajant ES1 or Cardinal on to a Boston Dynamics spot robot, with or without a GXP (General Expansion Payload). The standalone version allows the user to securely mount an ES1 to the robot, and provides networking to the robot as well as additional Ethernet and power outputs for additional payloads. Also included is a PoE+ output for powering and networking to a Fluke SV600. 

- GXP elimination circuitry (removes the need for customer to provide a GXP)
- Powers and provides mounting solution for Rajant ES1 and Rajant Cardinal
- Secondary PoE+ output for use with PoE+ devices such as Fluke SV600

![alt text](rrs_side_view.jpg "Robot PoE Switch - Spot")


# OEM version specifications

Intended for third party integration applications. The OEM option provides the following:

- 10/100 Mbps networking with 4 Ethernet ports (1 PoE capable).
- Mounting for Rajant Cardinal
- Low profile design 

![alt text](OEM_side1.jpeg "OEM")




# Risk Assessment

https://chick92.github.io/robot_poe_switch_instructions/Risk_Assessment_usage_switch.pdf

# Certifications

##### CE

https://chick92.github.io/robot_poe_switch_instructions//CE_robot_poe_switch.pdf

##### UKCA

https://chick92.github.io/robot_poe_switch_instructions//UKCE_Robot_PoE_Switch.pdf


# Warnings

- Do not disassemble device, warranty will be void if device is tampered with.
- Do not short power terminals
- Do not exceed the specified input voltage


# Spot Version


The following is provided with the standalone unit:

1x 15 cm Ethernet cable
4x M5 10 mm Hex bolts
4x M5 T nuts
2x M4 6 mm Hex bolts for Rajant ES1
2x M6 25 mm Hex bolts for Rajant Cardinal

# Mounting Rajant Cardinal or Rajant ES1

Rajant ES1 and Cardinal breadcrumbs can be mounted on to the top of the Robot PoE Switch, using the provided bolts. M4 for the ES1 and M6 for the Cardinal. 

![alt text](RPS_top.jpg "RPS_top")

Use only the bolts provided with the Robot PoE Switch as they are of a specified length.

Connect the Rajant Cardinal or ES1 to the Ethernet output labeled "Rajant". DO NOT connect it to the Silver Ethernet output labeled "PoE+" as this is an Active PoE output and WILL NOT power the Rajant.

![alt text](RPS_Rajant.jpg "Rajant PoE passive")

# Mounting on Spot

The Robot PoE Switch is designed to be mounted on the top of a Boston Dynamics spot, and as such is compatible with the payload rail spacing. Use the included M5 T-Nuts and M5 bolts. It is recommended to use loctite if available, and torque to hand-tight.

Once mounted, you will need to add the payload credentials to Spot

- Power on the robot, and log into the admin console using the admin credentials
- Go to the payload section and click "new custom payload"
- Enter "RobotPoESwitch" as the name
- Enter "OSE Rajant Robot PoE switch with ES1" as the description
- or X, Y and Z positions, enter -0.38, 0, 0.08 respectively. Note that if you're doing this on the Samsung Active Tab3 tablet, you'll need to use a notepad to type a "-" symbol, as at the time of writing Android 10 treats the field as number entry only.
- Enter 0,0,0 for Roll Pitch and Yaw
- Enter 0.5 kg for payload mass
- Enter 0,0,0 for position of centre of mass
- Leave as "point mass"

# Secondary PoE+ output

The Robot PoE Switch PoE+ output allows the user to power and network with additional PoE+ enabled sensors such as the Fluke SV600, without additional interface hardware. 
The PoE+ output is found at the rear of the device, above the payload interface cable. Simply connect an Ethernet cable from this port to your sensor. 

This output is labeled as PoE+. Do not connect the Rajant to this, as it will not work, and could potentially damage the Rajant. 

![alt text](RPS_PoE+.jpg "PoE+ output")


# OEM version mounting information

![alt text](OEM_measurements.png "Dimensions")