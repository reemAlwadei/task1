Mechanical Design of a Basic Robot Dog (Task 1)

This repository contains the initial mechanical design and architectural documentation for a basic robot dog. The main objective of this project is to understand the core mechanical principles that enable a quadruped robot to stand, balance, and walk.

Project Deliverables and Focus Areas

The design strictly covers the following fundamental engineering requirements based on the assignment guidelines:

1. Body Shape and Structure: Engineering the main chassis to house internal electronics and provide structural integrity.
2. Leg Design: Developing leg segments optimized for weight distribution and clearance.
3. Joints and Degrees of Freedom: Configuration of the joints to ensure proper locomotion flexibility.
4. Actuator Selection: Selecting proper servo motors based on torque requirements.
5. Initial Torque Calculations: Preliminary mathematical estimation of the torque required to support static and dynamic weight.
6. Stability and Center of Gravity: Analysis of the robot physical equilibrium to ensure it remains upright.
7. Proposed Locomotion Gait: Planning the gait cycle for stable displacement.
8. Anticipated Mechanical Issues: Identifying potential failure points such as backlash or friction losses.

Preliminary Torque Calculation Formulation

The static torque required at a joint can be estimated using the standard lever arm formula:

Torque = Force x Distance x Safety Factor

Where:
- Force: Is the force exerted due to the robot weight (Mass x Gravity).
- Distance: Is the effective perpendicular distance from the joint axis to the line of action of the force.
- Safety Factor: Recommended 1.5x to 2x to accommodate dynamic acceleration forces.

Core Objective

The target is not to build an ultra-advanced robotic system, but to thoroughly comprehend and implement the foundational mechanical physics that empower a robot to successfully execute stand and walk routines.



### Preliminary Torque Calculation

To calculate the preliminary torque required for the motors, a worst-case scenario was assumed where the robot's leg is fully extended horizontally, based on the actual design dimensions in Tinkercad.

**Formula Used:**
Torque = Force × Leg Length

**Actual Calculation Data:**
- Assumed Robot Mass: 1.5 kg
- Force acting on a single joint (assuming the load is distributed over two legs during walking): 7.35 N
- Actual Leg Length from the design: 0.031 m

**Substitution and Result:**
Torque = 7.35 × 0.031 = 0.228 N.m

The preliminary required torque per joint is 0.228 N.m, which falls within the appropriate range for small servo motors used in robots of this size to ensure balance and movement capability.


void walkForward() {
  // Simple gait pattern
  leg1.write(90); leg3.write(90); 
  delay(500);
  leg2.write(120); leg4.write(120); 
  delay(500);
}

Potential Mechanical Issues:

1. Center of Gravity: Instability caused by unbalanced weight distribution.
2. Torque Limitations: Servo motors failing to support the robot's total weight.
3. Friction Issues: Foot slippage on smooth surfaces due to lack of traction.
4. Mechanical Backlash: Gear slop in servos causing inaccurate leg positioning.
5. Power Instability: Voltage drops during motor movement triggering system resets.
