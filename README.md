
# Introduction
- This project combines the 3 Modes of mobility robot: Remoted controlled(RC), Line following, and Sumobot. it uses RC Tranceiver to select the robot modes.

# Technical information

### Controller and drivers
 For the controller, it utilizes 4 major components: 2 Arduino uno R3, Tranceiver module, and a sparkfun monster moto shield VNH2SP30. the first arduino uno will be responsible for sending commands to the second arduino uno via serial communication. the first arduino uno is responsible for 2 things: RC control, and M de selection. a type of communication called simplex communication is used since its only used is to send commands to the main arduino uno. it also has an 3 LED indicators, which will be used to indicate the current mode.

the second arduino(main) will handle the entire sensors in the mobot and the Motor driver, and uses the commands from the first arduino to control the modes via RC tranceiver.

-  Sensors

The sensors used in this project is the photoelectric sensor for line tracking and an E18-D80NK Proximity sensor for Distance detection. photoelectric sensors consists of 8 channels at the front and 1 each at the back corners(left and rignt). for digital interpretation of the lne tracking sensor, we use a LM339 voltage comparator to convert its analog output into digital. for LED indicators. it uses an OR gate, configured as buffer to drive the output of the voltage comparator because its output is open collector. both voltage comparator modules for front and back sensors are separated to make the wirings easier to connect. also, both sensors have independent Reference voltage for calibration

both LED indicators for 8 and 2 channel sensors are combined, including a tact switch for serial communication and the 2 independent reference voltage for calibrating the sensors in order for adjustments to be much more efficient when it comes to calibration and debugging.


-  Actuator

f

- Connection

for reliable contact, we use a JST XH connectos since it is easier when it comes to removing, or plugging the module in rather than using a jummper wires, which can be unreliable due to vibration.
