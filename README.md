
# Introduction
- This project combines the 3 Modes of mobility robot: Remoted controlled(RC), Line following, and Sumobot. it uses RC Tranceiver to select the robot modes.

# Technical information

### Controller
 For the controller, it utilizes 3 major components: 2 Arduino uno R3 and a Tranceiver module. the first arduino uno will be responsible for sending commands to the second arduino uno via serial communication. a method simplex communication is used since its only used is to send commands to the main arduino uno. it also has an 3 LED indicators, which will be used to inticate which mode is selected. 

-  Sensors

-  Actuator
