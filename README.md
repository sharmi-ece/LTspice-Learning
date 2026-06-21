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
