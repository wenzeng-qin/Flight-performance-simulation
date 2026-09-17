# Flight-performance-simulation
Development of a Python-based aircraft flight-performance simulation tool. 

Sidenote: You maybe have noticed that this entire project is written in Jupyter Notebook file instead of the conventional .py script, this is because I work with mathematical and physical model most of the time, Jupyter notebook has became my main go to option for any python project and its also just easier for me to set up my environment in .pynb format for the IDE I used to program this.

## Claim
This project is developed out of my own interest for aircraft simulation before taking any formal course in numerical analysis at school. It served as a good practice in building the physics engine from first principle and using data analysis tools for automated testing. The coding of the the physics engine is build under my own knowledge and research of atmospheric physics and python where I have intentionally limited the use of AI until the very last of the validation stage of the project to speed up with data collection and verifying the realism of the model. There are some interest finding here which I will discuss in detail.

---

## Verdict on the result

Something interest I find from the result comparison during the validation stage is how the error result from my simplified assumption lead to the deviation of shape of the flight envelope.

## Project Goals

The simulator will be developed to model:

* Atmospheric conditions at different altitudes
* Lift and drag
* Aircraft stall speed
* Engine thrust
* Thrust and drag relationships
* Climb performance
* Aircraft acceleration
* Flight envelope
* Time-dependent flight behaviour

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

---

## File Structure

```text
aircraft-performance-simulator/
│
├── src/
│   ├── atmosphere.py
│   ├── aerodynamics.py
│   ├── propulsion.py
│   └── simulation.py
│
├── tests/
│
│
├── results/
│
├── README.md
└── requirements.txt
```

---

## Tools

* Python
* NumPy
* SciPy
* Matplotlib
* Pandas

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

