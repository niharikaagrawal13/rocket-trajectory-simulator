# Rocket Trajectory Simulator

A Python-based numerical simulation to model the vertical ascent of a rocket. This project integrates physics modeling with numerical methods to analyze the impact of design parameters on flight performance.

## Project Overview

I developed a 3-DOF physics simulator from the ground up to analyze rocket performance. The core purpose was to investigate the complex interplay between design parameters and their real-world effects on flight outcomes.

## Key Features & Physics Modeled

- **Numerical Integration:** Solved equations of motion using Euler's method.
- **Forces Modeled:** Thrust (with finite burn time), Gravitational Force, Aerodynamic Drag.
- **Outputs:** Plots for altitude, velocity, acceleration, mass, and dynamic pressure.

## Physics Investigations

### 1. Burnout Acceleration Spike Analysis
- **Observation:** Identified a massive negative acceleration spike at engine cutoff.
- **Conclusion:** The spike is caused by the sudden loss of thrust occurring simultaneously with the rocket's minimum mass, leaving only large downward forces to act on a lightweight airframe.

### 2. Thrust vs. Performance Trade-off
- **Hypothesis:** A 25% increase in thrust would significantly increase apogee.
- **Result:** Confirmed higher thrust yielded higher velocity and altitude.
- **Key Insight:** Discovered a major trade-off: the higher thrust led to a more severe acceleration spike at burnout due to exponentially increased drag forces from the higher velocity.

## How to Run

1.  Open the `rocket_simulator.ipynb` Jupyter Notebook.
2.  Run all cells sequentially to see the simulation and analysis.
