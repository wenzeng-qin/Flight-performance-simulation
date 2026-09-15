# Flight-performance-simulation
Development of a Python-based aircraft flight-performance simulation tool.

The aim of this project is to combine aerodynamics, physics, numerical methods and Python programming to create a simple aircraft performance simulator.

## Project Goals

The simulator will progressively be developed to model:

* Atmospheric conditions at different altitudes
* Lift and drag
* Aircraft stall speed
* Engine thrust
* Thrust and drag relationships
* Climb performance
* Aircraft acceleration
* Flight envelope
* Time-dependent flight behaviour

The project will also use numerical methods to solve engineering problems that cannot easily be solved analytically.

---

## Project Development

### 1. Atmosphere Model

Create a model that calculates atmospheric temperature, pressure and density at different altitudes.

The results will be visualised to investigate how atmospheric conditions change with altitude.

### 2. Aerodynamic Model

Implement simplified models for aircraft lift and drag.

The model will be used to investigate how aerodynamic forces change with:

* Airspeed
* Air density
* Angle of attack
* Aircraft configuration

### 3. Aircraft Model

Create an aircraft model containing parameters such as:

* Mass
* Wing area
* Aspect ratio
* Maximum lift coefficient
* Drag parameters
* Engine thrust

### 4. Stall Speed

Use the aerodynamic model to calculate stall speed and investigate how it changes with:

* Aircraft mass
* Altitude
* Maximum lift coefficient

### 5. Engine Model

Implement a simplified engine thrust model.

The initial model will focus on how available thrust changes with altitude, velocity and throttle rather than attempting to reproduce the detailed thermodynamics of a real engine.

### 6. Aircraft Performance

Compare available thrust with aerodynamic drag to investigate:

* Equilibrium speeds
* Maximum speed
* Excess thrust
* Acceleration

Numerical root-finding methods will be used to solve for equilibrium conditions.

### 7. Climb Performance

Calculate aircraft rate of climb and investigate how climb performance changes with:

* Altitude
* Airspeed
* Aircraft mass
* Throttle

### 8. Flight Simulation

Introduce ordinary differential equations to simulate aircraft motion over time.

This will allow scenarios such as acceleration and climbing to be simulated numerically.

### 9. Flight Envelope

Use the performance model to estimate the range of speeds available to the aircraft at different altitudes.

The results will be visualised as a flight-envelope diagram.

### 10. Validation

The final model will be compared against published performance data from a real aircraft.

Differences between the model and reference data will be analysed to identify limitations in the simplified model.

---

## Numerical Methods

Numerical methods will be used throughout the project, including:

* Root finding
* Numerical integration
* Optimisation
* Interpolation
* Error analysis

Where appropriate, numerical algorithms will be implemented and compared with methods provided by scientific Python libraries.

---

## Software Structure

```text
aircraft-performance-simulator/
│
├── src/
│   ├── atmosphere.py
│   ├── aerodynamics.py
│   ├── propulsion.py
│   ├── aircraft.py
│   └── simulation.py
│
├── tests/
│
├── notebooks/
│
├── results/
│
├── README.md
└── requirements.txt
```

---

## Technologies

* Python
* NumPy
* SciPy
* Matplotlib
* Pandas
* pytest
* Git/GitHub

---

## Current Status

This project is currently under development.

* [ ] Atmosphere model
* [ ] Aerodynamic model
* [ ] Aircraft model
* [ ] Stall-speed calculation
* [ ] Engine model
* [ ] Thrust/drag analysis
* [ ] Numerical root finding
* [ ] Climb performance
* [ ] Flight simulation
* [ ] Flight envelope
* [ ] Real-aircraft validation
* [ ] Automated testing

---

## Future Development

Possible future improvements include:

* More realistic engine modelling
* Mach-number-dependent aerodynamics
* Improved atmospheric modelling
* Wind and atmospheric disturbances
* More complete aircraft dynamics
* Control-surface modelling
* Sensitivity analysis
* Comparison with CFD results
* Integration with OpenFOAM

---

## Project Motivation

This project is intended to develop practical engineering programming skills by applying Python to a real aerospace engineering problem.

The focus is on building a model from physical principles, solving it numerically, analysing the results, and understanding the limitations of the model.
