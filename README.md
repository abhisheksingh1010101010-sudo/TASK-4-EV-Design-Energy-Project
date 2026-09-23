# TASK-4-EV-Design-Energy-Project
Electric Vehicle Technology Internship
Project Title

Basic Electric Vehicle Design and Energy Consumption Analysis

1. Introduction

Electric Vehicles (EVs) are becoming an important part of modern transportation because they offer higher energy efficiency and can reduce dependence on conventional fossil fuels. An EV mainly consists of a battery pack, electric motor, motor controller/inverter, Battery Management System (BMS), charging system, and vehicle control system.

In this project, a basic electric vehicle system is designed for a small urban electric car. The objective is to estimate the required battery capacity, motor power, approximate driving range, and energy consumption under different operating conditions.

The design is based on practical engineering assumptions and simplified calculations suitable for an academic EV design study.

2. Selected Vehicle/Application

For this project, the selected application is:

Vehicle: Small Urban Electric Car
Application: City transportation and short-distance commuting

Assumed Vehicle Specifications
Parameter	Assumed Value
Vehicle type	Small Urban EV
Kerb mass	900 kg
Passengers	2
Total loaded mass	1050 kg
Maximum speed	80 km/h
Typical city speed	40 km/h
Battery voltage	144 V
Battery capacity	30 kWh
Motor type	Permanent Magnet Synchronous Motor
Motor peak power	40 kW
Motor continuous power	20 kW
Drivetrain efficiency	90%
Battery usable SOC range	90%
Estimated practical range	~180 km
3. Basic EV System Design

The proposed EV consists of the following major components:

1. Battery Pack

The battery is the primary energy storage unit of the vehicle. A 30 kWh lithium-ion battery pack is selected for this design.

2. Electric Motor

A 40 kW PMSM motor is selected because it provides good efficiency and suitable torque characteristics for an urban EV.

3. Motor Controller/Inverter

The inverter converts the battery's DC electrical power into the required AC power for the motor and controls motor speed and torque.

4. Battery Management System (BMS)

The BMS monitors:

Cell voltage
Battery current
Temperature
State of Charge (SOC)
Battery protection conditions
5. Charging System

An onboard AC charger can be used for normal charging, while DC fast charging can be used where supported.

6. Transmission/Reduction Gear

A single-speed reduction gearbox transfers motor torque to the driving wheels.

7. Regenerative Braking

During deceleration, the motor can operate as a generator and recover part of the vehicle's kinetic energy back into the battery.

4. Basic EV System Block Diagram

Battery Pack → BMS → Inverter/Controller → Electric Motor → Reduction Gear → Wheels

Additional systems:

Charging Station → Onboard Charger → Battery

Wheels → Regenerative Braking → Motor → Inverter → Battery

5. Battery Capacity Estimation

The selected battery capacity is:

Battery Capacity = 30 kWh

Assuming the usable battery SOC window is approximately 90%:

Usable Energy = 30 × 0.90

Usable Energy = 27 kWh

Therefore, approximately 27 kWh of the battery's nominal energy can be considered usable for normal operation.

6. Battery Pack Voltage and Ah Capacity

The battery voltage is assumed to be:

V = 144 V

Battery energy:

E = 30 kWh = 30,000 Wh

Battery capacity in Ah can be estimated using:

Capacity (Ah) = Energy (Wh) / Voltage (V)

Therefore:

Capacity = 30,000 / 144

Capacity ≈ 208.3 Ah

So the proposed battery pack is approximately:

144 V, 208 Ah, 30 kWh

7. Motor Requirement

The vehicle requires sufficient motor power for:

Starting from rest
Acceleration
Climbing gradients
Maintaining cruising speed
Overcoming aerodynamic and rolling resistance

For this project, a:

40 kW peak PMSM motor

is selected.

A continuous rating of approximately:

20 kW

is considered sufficient for normal urban driving.

The peak rating provides additional power during acceleration and hill climbing.

8. Approximate Range Calculation

Assume the estimated average energy consumption is:

150 Wh/km

Usable battery energy:

27,000 Wh

Therefore:

Range = Usable Battery Energy / Energy Consumption

Range = 27,000 / 150

Range ≈ 180 km

Therefore, the estimated practical driving range under the assumed conditions is approximately:

180 km per charge

Actual range will vary depending on speed, traffic, road conditions, vehicle load, temperature, driving style, and use of auxiliary systems such as air conditioning.

9. Energy Consumption Under Different Conditions

Energy consumption changes according to the operating conditions of the vehicle.

Driving Condition	Approx. Consumption	Estimated Range*
Slow city traffic	130 Wh/km	~208 km
Normal city driving	150 Wh/km	~180 km
Highway driving	180 Wh/km	~150 km
High-speed driving	220 Wh/km	~123 km
Heavy load / frequent acceleration	200 Wh/km	~135 km

*Range values are theoretical estimates based on 27 kWh usable energy.

10. Energy Consumption Calculation

For normal city driving:

Energy consumption = 150 Wh/km

For a distance of 100 km:

Energy required = 150 × 100

= 15,000 Wh

= 15 kWh

Therefore, approximately 15 kWh of usable battery energy would be required for 100 km under the assumed normal-city-driving condition.

11. Motor Power and Battery Power

The motor's peak mechanical power is:

40 kW

Assuming drivetrain efficiency of approximately 90%:

Battery input power = Motor output power / Efficiency

= 40 / 0.90

≈ 44.4 kW

Therefore, when the motor is delivering approximately 40 kW mechanically, the battery-side electrical power requirement can be around 44.4 kW, excluding other auxiliary electrical loads.

This demonstrates why the battery, inverter, cables, and protection systems must be designed to handle high current during acceleration.

12. Energy Consumption Factors

The energy consumption of an EV depends on several factors:

A. Vehicle Weight

Higher vehicle mass requires more energy during acceleration.

B. Speed

At higher speeds, aerodynamic drag increases significantly, increasing energy consumption.

C. Road Gradient

Driving uphill requires additional power because the vehicle must overcome gravitational force.

D. Driving Style

Frequent acceleration and braking generally increase energy consumption.

E. Tire Pressure

Incorrect tire pressure can increase rolling resistance and reduce efficiency.

F. Weather Conditions

Temperature can affect battery performance and energy consumption.

G. Auxiliary Loads

Air conditioning, heating, lighting, and infotainment systems also consume electrical energy.

13. Regenerative Braking

Regenerative braking is an important feature of electric vehicles.

During braking:

Vehicle Kinetic Energy → Electric Motor → Electrical Energy → Battery

Instead of converting all braking energy into heat through conventional friction brakes, part of the kinetic energy can be recovered and stored in the battery.

However, regenerative braking does not recover 100% of the energy because losses occur in the motor, inverter, battery, and mechanical system.

14. Technical Justification of the Design

The proposed specifications are selected to provide a balance between performance, battery capacity, vehicle weight, range, and efficiency.

30 kWh Battery

A 30 kWh battery provides sufficient energy for an estimated ~180 km range under the assumed normal city-driving consumption.

40 kW Motor

A 40 kW peak motor provides adequate power for a small urban vehicle while allowing additional power for acceleration and gradients.

144 V Battery System

The selected voltage provides a reasonable balance between current requirements and system complexity for this conceptual design.

PMSM Motor

PMSM motors are suitable for EV applications because of their high efficiency, compact size, and good torque characteristics.

15. Advantages of the Proposed EV Design
Zero tailpipe emissions during operation
High electric drivetrain efficiency
Lower energy consumption compared with many conventional vehicles
Regenerative braking capability
Reduced dependence on fossil fuels
Suitable for urban transportation
Simple single-speed drivetrain
Potentially lower routine maintenance requirements
16. Limitations and Assumptions

This project is a conceptual engineering design, so the calculations are based on assumed values.

Actual EV performance would require detailed analysis of:

Battery cell chemistry
Cell configuration
Thermal management
Motor torque-speed characteristics
Vehicle aerodynamics
Tire specifications
Road gradient
Drive-cycle testing
Inverter losses
Auxiliary loads
Battery aging

Therefore, the calculated range should be considered an approximate engineering estimate rather than a certified vehicle specification.

17. Final Design Summary
Component	Proposed Specification
Vehicle	Small Urban Electric Car
Total loaded mass	1050 kg
Battery	30 kWh Lithium-ion
Battery voltage	144 V
Approx. battery capacity	208 Ah
Motor	PMSM
Peak motor power	40 kW
Continuous motor power	20 kW
Drivetrain efficiency	90%
Usable battery energy	27 kWh
Normal energy consumption	~150 Wh/km
Estimated range	~180 km
Maximum speed	~80 km/h
Regenerative braking	Yes
18. Conclusion

This project provided a practical understanding of how the major components of an Electric Vehicle system are selected and how battery capacity, motor power, energy consumption, and driving range are related.

For the proposed small urban EV, a 30 kWh battery pack and 40 kW peak PMSM motor were selected. Based on an assumed normal energy consumption of approximately 150 Wh/km, the estimated range is around 180 km using approximately 27 kWh of usable battery energy.

The analysis demonstrates that EV design is a system-level engineering problem in which battery capacity, motor power, efficiency, vehicle mass, speed, road conditions, and driving patterns all influence vehicle performance.

Skills/Knowledge Gained
EV system architecture
Battery capacity calculation
Motor power estimation
Energy consumption analysis
Driving-range estimation
Regenerative braking concepts
Basic EV component selection
Technical documentation and engineering calculations

Project Outcome:
A basic conceptual EV system was successfully designed with estimated battery capacity, motor requirement, driving range, and energy consumption under different operating conditions.
