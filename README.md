TASK 4: EV DESIGN & ENERGY PROJECT
Project Title

Design and Energy Analysis of a Battery Electric Vehicle (BEV)

Internship Domain

Electric Vehicle Technology

Project Objective

The objective of this project is to design a basic electric vehicle system for a selected vehicle application and estimate its motor power, battery capacity, energy consumption and driving range. The project also analyzes the energy requirement of the vehicle under different operating conditions such as city driving, highway driving, acceleration and uphill driving.

1. Selected Vehicle/Application

For this project, a compact electric passenger car is selected.

The vehicle is designed for daily urban and highway transportation with a practical balance between performance, battery capacity and driving range.

Basic Vehicle Specification

| Parameter                         |                       Design Value |
| --------------------------------- | ---------------------------------: |
| Vehicle type                      |               Compact Electric Car |
| Number of passengers              |                                  4 |
| Vehicle mass                      |                            1200 kg |
| Maximum speed                     |                           100 km/h |
| Target cruising speed             |                            60 km/h |
| Aerodynamic drag coefficient (Cd) |                               0.29 |
| Frontal area                      |                             2.2 m² |
| Rolling resistance coefficient    |                              0.012 |
| Wheel radius                      |                             0.29 m |
| Drivetrain efficiency             |                                90% |
| Battery nominal voltage           |                              350 V |
| Battery capacity                  |                             30 kWh |
| Motor type                        | Permanent Magnet Synchronous Motor |
| Motor peak power                  |                              50 kW |
| Motor continuous power            |                           25–30 kW |
| Estimated practical range         |                        ~180–200 km |

2. Basic EV System Architecture

The proposed EV consists of the following major components:

Battery Pack → Inverter → Electric Motor → Transmission → Wheels

Additional systems include:

Battery Management System (BMS)
On-board charger
DC-DC converter
Vehicle Control Unit (VCU)
Regenerative braking system
Thermal management system
Charging port
Working Principle

The battery stores electrical energy in DC form. The inverter converts the battery's DC power into controlled AC power for the traction motor. The motor converts electrical energy into mechanical torque, which is transferred to the wheels through the reduction gearbox.

During braking, the motor can operate as a generator and recover part of the vehicle's kinetic energy. This energy is returned to the battery through the regenerative braking system.

3. Vehicle Forces

The main forces acting against an EV during motion are:

Rolling resistance
Aerodynamic drag
Gradient resistance
Acceleration force

The total tractive force required is:

$$ F_{total}=F_{rolling}+F_{aero}+F_{grade}+F_{acceleration} $$
4. Rolling Resistance

Rolling resistance is given by:

$$ F_{rolling}=C_{rr}mg $$

Where:

\(C_{rr}=0.012\)
\(m=1200\,kg\)
\(g=9.81\,m/s^2\)

Therefore:

$$ F_{rolling}=0.012\times1200\times9.81 $$ $$ \boxed{F_{rolling}=141.3\,N} $$

So approximately 141 N of force is required to overcome rolling resistance on a flat road.

5. Aerodynamic Drag

Aerodynamic resistance is:

$$ F_{aero}=\frac{1}{2}\rho C_d A v^2 $$

Assume:

Air density, \(\rho=1.225\,kg/m^3\)
\(C_d=0.29\)
\(A=2.2\,m^2\)

At 60 km/h:

$$ v=\frac{60}{3.6}=16.67\,m/s $$

Therefore:

$$ F_{aero}=\frac12(1.225)(0.29)(2.2)(16.67)^2 $$ $$ \boxed{F_{aero}\approx122\,N} $$
6. Power Requirement at 60 km/h

At 60 km/h on a level road:

$$ F_{total}=141.3+122 $$ $$ F_{total}\approx263.3\,N $$

Vehicle speed:

$$ v=16.67\,m/s $$

Mechanical power required:

$$ P=Fv $$ $$ P=263.3\times16.67 $$ $$ P\approx4388\,W $$

Therefore:

$$ \boxed{P_{wheel}\approx4.4\,kW} $$

Considering 90% drivetrain efficiency:

$$ P_{battery}=\frac{4.4}{0.90} $$ $$ \boxed{P_{battery}\approx4.9\,kW} $$

Thus, approximately 4.9 kW electrical power is required to maintain 60 km/h on a level road under these assumptions.

7. Motor Power Requirement

The motor must provide enough power for:

Normal cruising
Acceleration
Uphill driving
Overtaking
Additional load
Real-world losses

Although the calculated cruising power is relatively low, a substantially higher motor rating is required for acceleration and gradients.

Selected Motor

50 kW peak PMSM traction motor

Specifications:

| Parameter        |                                          Value |
| ---------------- | ---------------------------------------------: |
| Motor type       |                                           PMSM |
| Peak power       |                                          50 kW |
| Continuous power |                                       25–30 kW |
| Nominal voltage  |                                         ~350 V |
| Maximum speed    |                                    ~10,000 rpm |
| Application      |                                       Traction |
| Cooling          | Liquid/air cooling depending on implementation |


A 50 kW peak motor provides a reasonable margin over the calculated normal cruising requirement.

8. Motor Torque Requirement

Wheel torque can be calculated from:

$$ T=F\times r $$

For level-road cruising at 60 km/h:

$$ T=263.3\times0.29 $$ $$ \boxed{T\approx76\,Nm} $$

However, the actual motor must provide considerably higher torque during vehicle launch and acceleration.

With a reduction gearbox, the motor torque can be multiplied before reaching the wheels.

For example, assuming a reduction ratio of approximately 9:1, the required motor torque is reduced compared with direct drive.

9. Acceleration Requirement

Suppose the vehicle is required to accelerate from:

0 to 50 km/h in 10 seconds

Final velocity:

$$ 50/3.6=13.89\,m/s $$

Average acceleration:

$$ a=\frac{13.89}{10} $$ $$ a=1.389\,m/s^2 $$

Acceleration force:

$$ F_{acc}=ma $$ $$ F_{acc}=1200\times1.389 $$ $$ \boxed{F_{acc}\approx1667\,N} $$

Adding rolling and aerodynamic resistance, the total force during acceleration is approximately:

$$ F_{total}\approx1667+141+85 $$ $$ \boxed{F_{total}\approx1893\,N} $$

At 50 km/h:

$$ P=Fv $$ $$ P=1893\times13.89 $$ $$ P\approx26.3\,kW $$

Considering drivetrain losses, approximately:

$$ P_{battery}\approx\frac{26.3}{0.90} $$ $$ \boxed{P_{battery}\approx29.2\,kW} $$

Therefore, a 50 kW peak motor provides sufficient power margin for the assumed acceleration requirement.

10. Uphill/Gradient Analysis

Consider a 5% road gradient.

Gradient force:

$$ F_{grade}=mg\times0.05 $$ $$ F_{grade}=1200\times9.81\times0.05 $$ $$ \boxed{F_{grade}\approx589\,N} $$

At 60 km/h, total force becomes approximately:

$$ F_{total}=141+122+589 $$ $$ \boxed{F_{total}\approx852\,N} $$

Required wheel power:

$$ P=852\times16.67 $$ $$ P\approx14.2\,kW $$

Battery power considering 90% efficiency:

$$ P_{battery}=\frac{14.2}{0.9} $$ $$ \boxed{P_{battery}\approx15.8\,kW} $$

Therefore, the selected 50 kW motor can comfortably provide the required power for this operating condition.

11. Battery Design

For the proposed vehicle, a 30 kWh lithium-ion battery pack is selected.

| Parameter                   |                     Value |
| --------------------------- | ------------------------: |
| Battery chemistry           |               Lithium-ion |
| Nominal voltage             |                     350 V |
| Capacity                    |                    30 kWh |
| Approximate usable capacity |                    27 kWh |
| Battery management          |                       BMS |
| Cooling                     | Thermal management system |
| Charging                    |               AC charging |
| Regenerative braking        |                       Yes |


The usable battery capacity is assumed to be around 90% of the nominal capacity to avoid operating continuously at the extreme ends of the battery's state of charge.

$$ 30\times0.90=27\,kWh $$

Thus:

$$ \boxed{E_{usable}\approx27\,kWh} $$
12. Battery Ah Capacity

Battery capacity in Ah can be estimated using:

$$ Ah=\frac{Wh}{V} $$ $$ Ah=\frac{30,000}{350} $$ $$ \boxed{Ah\approx85.7\,Ah} $$

Therefore, the proposed battery pack is approximately:

350 V, 86 Ah, 30 kWh

13. Estimated Energy Consumption

For practical estimation, an average energy consumption of approximately:

$$ \boxed{150\,Wh/km} $$

is assumed for mixed driving.

This includes energy used for:

Motor
Inverter
Transmission
Rolling resistance
Aerodynamic losses
Auxiliary systems
Real-world operating losses
14. Estimated Driving Range

Using usable battery energy:

$$ Range=\frac{Battery\ Energy}{Energy\ Consumption} $$ $$ Range=\frac{27,000}{150} $$ $$ \boxed{Range\approx180\,km} $$

Using the full nominal battery capacity:

$$ Range=\frac{30,000}{150} $$ $$ \boxed{Range\approx200\,km} $$

Therefore, the expected practical range is approximately:

180–200 km per charge

Actual range would vary with speed, temperature, road gradient, traffic, payload, tyre pressure and driving style.

15. Energy Consumption Under Different Conditions
Driving Condition	Approx. Consumption
Low-speed city driving	130–160 Wh/km
Normal mixed driving	~150 Wh/km
Highway driving	160–190 Wh/km
High-speed driving	190–230 Wh/km
Uphill driving	220–300+ Wh/km
Heavy traffic with frequent acceleration	170–210 Wh/km

These values are engineering estimates for the proposed design rather than measured test results.

16. Range Under Different Conditions

Using a usable battery capacity of approximately 27 kWh:

City

Assume:

$$ 150\,Wh/km $$ $$ Range=\frac{27000}{150} $$ $$ \boxed{180\,km} $$
Highway

Assume:

$$ 180\,Wh/km $$ $$ Range=\frac{27000}{180} $$ $$ \boxed{150\,km} $$
High-Speed Driving

Assume:

$$ 210\,Wh/km $$ $$ Range=\frac{27000}{210} $$ $$ \boxed{129\,km} $$

Thus, driving conditions have a significant effect on EV range.

17. Regenerative Braking

Regenerative braking is an important feature of the proposed EV.

During conventional braking, kinetic energy is mostly converted into heat through the braking system. In regenerative braking, the traction motor operates as a generator.

Energy Flow

Vehicle kinetic energy → Motor/Generator → Inverter → Battery

Regenerative braking can recover a portion of the energy that would otherwise be lost.

However, the actual recovered energy depends on:

Vehicle speed
Braking intensity
Battery state of charge
Motor efficiency
Road conditions
Control strategy
18. Charging Requirement

For a 30 kWh battery, assuming an AC charging power of 7.2 kW:

$$ Charging\ Time=\frac{30}{7.2} $$ $$ \boxed{\approx4.2\ hours} $$

Considering charging losses, practical charging time would be somewhat higher.

Proposed Charging System
AC charging: approximately 7.2 kW
Battery: 30 kWh
Charging time: approximately 4–5 hours
Charging interface: suitable EV AC charging connector
BMS-controlled charging
19. Major Components of Proposed EV
1. Battery Pack

Stores electrical energy and supplies power to the vehicle.

2. Battery Management System

Monitors:

Voltage
Current
Temperature
State of Charge
Cell balancing
Battery protection
3. Inverter

Converts DC battery power into controlled AC power for the motor.

4. PMSM Motor

Converts electrical energy into mechanical energy.

5. Reduction Gearbox

Transfers motor torque to the wheels while providing the required speed reduction.

6. DC-DC Converter

Converts high-voltage battery power to low voltage for auxiliary electrical systems.

7. On-Board Charger

Converts AC charging power into DC power suitable for the battery.

8. Vehicle Control Unit

Coordinates motor control, battery management, braking and other vehicle functions.

20. Overall Energy Flow
              AC GRID
             │
             ▼
      ON-BOARD CHARGER
             │
             ▼
       BATTERY PACK
             │
             ▼
            BMS
             │
             ▼
          INVERTER
             │
             ▼
      PMSM ELECTRIC MOTOR
             │
             ▼
       REDUCTION GEAR
             │
             ▼
           WHEELS
             │
             ▼
          VEHICLE

During regenerative braking:
 WHEELS
   ↓
ELECTRIC MOTOR
   ↓
INVERTER
   ↓
BATTERY
21. Design Summary
| Parameter                 | Final Design |
| ------------------------- | -----------: |
| Vehicle                   |   Compact EV |
| Vehicle mass              |      1200 kg |
| Maximum speed             |     100 km/h |
| Cruising speed            |      60 km/h |
| Motor                     |         PMSM |
| Motor peak power          |        50 kW |
| Motor continuous power    |     25–30 kW |
| Battery voltage           |        350 V |
| Battery capacity          |       30 kWh |
| Usable energy             |      ~27 kWh |
| Battery capacity          |       ~86 Ah |
| Energy consumption        |   ~150 Wh/km |
| Estimated practical range |   180–200 km |
| Drivetrain efficiency     |          90% |
| Charging power            |   ~7.2 kW AC |
| Approx. charging time     |    4–5 hours |
| Regenerative braking      |          Yes |

22. Technical Justification

The proposed EV design uses a 50 kW PMSM motor because the vehicle requires significantly more power during acceleration and uphill driving than during constant-speed cruising.

A 30 kWh lithium-ion battery is selected because it provides a practical balance between vehicle range, battery weight and cost. With an assumed average energy consumption of approximately 150 Wh/km, the vehicle can achieve an estimated practical range of around 180 km using 90% usable battery capacity.

The aerodynamic drag and rolling resistance calculations show that cruising on a level road requires considerably less power than acceleration. This demonstrates why motor sizing must consider transient conditions rather than only steady-state cruising.

The inclusion of regenerative braking can further improve overall energy efficiency by recovering a portion of the vehicle's kinetic energy during deceleration.

23. Conclusion

This project presents the conceptual design and energy analysis of a compact battery electric vehicle. Based on the selected vehicle parameters, a 50 kW PMSM traction motor and 30 kWh lithium-ion battery pack are proposed.

The calculated results indicate that approximately 4.9 kW of battery power is required for steady 60 km/h cruising on a level road under the stated assumptions, while approximately 15.8 kW may be required at 60 km/h on a 5% gradient. The acceleration analysis indicates a requirement of approximately 29 kW battery power for the assumed 0–50 km/h in 10 seconds condition.

With approximately 27 kWh usable battery energy and an assumed average consumption of 150 Wh/km, the estimated practical driving range is approximately 180 km, with the nominal-energy calculation giving approximately 200 km. Actual range will depend on speed, traffic, payload, temperature, terrain and driving conditions.

Overall, the proposed design demonstrates the basic engineering approach used in EV system design, including motor sizing, battery sizing, energy consumption estimation, range calculation, regenerative braking and charging requirements.
