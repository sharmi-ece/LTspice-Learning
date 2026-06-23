# LTspice-Learning
Learning LTspice through circuit simulation projects and electronics fundamentals.

This repository contains my LTspice learning projects and circuit simulations.

## Project 01: LED Circuit Simulation

### Objective

To design and simulate a basic LED circuit using LTspice and understand the relationship between voltage, current, and resistance.

### Components Used

* 5V DC Voltage Source
* 220Ω Resistor
* LED
* Ground

### Simulation Results

* Supply Voltage: 5V
* LED Forward Voltage: 0.73V
* LED Current: 19.4mA

### Learning Outcomes

* Created a schematic in LTspice
* Assigned component values
* Connected circuit components
* Performed DC Operating Point Analysis
* Observed voltage and current in a simple LED circuit

### Conclusion

The circuit was successfully simulated in LTspice. The resistor limited the current through the LED, and the simulation results confirmed normal LED operation.


## Project 02: ESP32 Battery Voltage Monitoring Using Voltage Divider

### Objective

To design and simulate a voltage divider circuit for monitoring a 12V battery using an ESP32 ADC input.

### Components Used

* 12V DC Voltage Source
* 27kΩ Resistor
* 10kΩ Resistor
* Ground

### Circuit Description

A voltage divider circuit was designed using 27kΩ and 10kΩ resistors to reduce the 12V battery voltage to a safe level for ESP32 ADC measurement.

### Simulation Results

* Input Voltage: 12V
* Output Voltage (Vout): 3.24V

### Learning Outcome

* Understood the working of a voltage divider.
* Learned how to scale voltages for microcontroller ADC inputs.
* Practiced LTspice circuit simulation and result analysis.
* Applied a real-world battery monitoring concept used in embedded systems.

### Conclusion

The voltage divider successfully reduced the 12V battery voltage to approximately 3.24V, making it suitable for ESP32 ADC measurement. This circuit can be used in battery monitoring applications for embedded and robotics projects.



## Project 03: Transistor as a Switch

### Aim

To understand the operation of an NPN transistor as an electronic switch and learn how a small control signal can control a larger load current.

### Objective

To design and simulate a transistor switching circuit in LTspice and analyze the relationship between Base Current (Ib), Collector Current (Ic), and Emitter Current (Ie).

### Components Used

* NPN Transistor
* LED
* 220Ω Resistor
* 1kΩ Base Resistor
* Two 5V DC Voltage Sources
* Ground

### Why Are Two Voltage Sources Used?

This was one of the key concepts learned during the project.

#### Voltage Source V1 (Power Source)

V1 supplies power to the load (LED). The current flows through the resistor, LED, transistor, and finally to ground.

#### Voltage Source V2 (Control Signal)

V2 provides a control signal to the transistor Base through a 1kΩ resistor. In a real embedded system, this voltage source represents a GPIO output from a microcontroller such as an ESP32.

The transistor allows a small control signal at the Base to control a larger current flowing through the Collector and Emitter.

### Circuit Working

When V2 provides 5V to the Base:

1. Base current flows through the 1kΩ resistor.
2. The transistor turns ON.
3. Current flows from V1 through the LED and transistor.
4. The LED glows.

When the Base signal is removed:

1. Base current becomes zero.
2. The transistor turns OFF.
3. No collector current flows.
4. The LED turns OFF.

### Simulation Results

Operating Point Results:

* Base Current (Ib) = 4.14 mA
* Collector Current (Ic) = 19.17 mA
* Emitter Current (Ie) = 23.31 mA
* LED Current = 19.17 mA

### Important Observation

A small Base current of approximately 4.14 mA controlled a larger Collector current of approximately 19.17 mA.

This demonstrates the switching and current amplification capability of a transistor.

Another important relationship observed during the simulation was:

Emitter Current = Base Current + Collector Current

This is one of the fundamental transistor relationships.

### Advantages

* Allows low-power devices to control higher-power loads.
* Fast switching operation.
* Low cost and widely available.
* Essential building block in embedded systems and robotics.

### Disadvantages

* Requires proper resistor selection.
* Current handling capability is limited by transistor ratings.
* Excess current can damage the transistor.

### Real-World Applications

* ESP32 controlled LEDs
* Relay driver circuits
* Motor control circuits
* Buzzer control circuits
* IoT devices
* Robotics applications
* Battery-powered embedded systems

### Learning Outcome

Through this project, I learned:

* The function of Base, Collector, and Emitter terminals.
* Why a Base resistor is required.
* Why separate power and control signals are used.
* How a transistor acts as an electronic switch.
* How microcontrollers control external loads using transistors.
* How to analyze LTspice operating point results.

### Conclusion

The LTspice simulation successfully demonstrated the operation of an NPN transistor as a switch. The project showed how a small control current can control a larger load current, which is a fundamental concept used in embedded systems, IoT devices, automation systems, and robotics.
