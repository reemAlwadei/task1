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
