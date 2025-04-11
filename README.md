# NeuronalDynamics-Simulation

## Overview
This repository contains a comprehensive implementation of computational neuroscience models for simulating neuronal dynamics. The project focuses on implementing the FitzHugh-Nagumo model, a simplified representation of action potentials in neurons, and optimizing its parameters using empirical neurophysiological data.

## Features
- Implementation of the FitzHugh-Nagumo model for neuronal dynamics
- First-order and second-order differential equation solvers
- Parameter optimization using real neuronal electrophysiology data
- Comparative analysis of different neuronal modeling techniques
- Interactive visualizations of neuronal responses to various stimuli

## Data Sources
The empirical neuronal data used in this project can be downloaded from:
- [Allen Brain Atlas - Cell Types](https://celltypes.brain-map.org/experiment/electrophysiology/474626527)

A helper script for downloading the data is included in the notebooks directory.

## Implemented Models
1. **FitzHugh-Nagumo Model** - A simplified two-dimensional model that captures the essential dynamics of neuronal action potentials:
   ```
   dv/dt = v - v³/3 - w + I
   dw/dt = ε(v + a - b·w)
   ```
   where:
   - v represents the membrane potential
   - w represents a recovery variable
   - I is the input current stimulus
   - ε, a, and b are parameters that control the model's behavior

## Results
The repository includes visualizations comparing the model's predictions with empirical data, parameter sensitivity analysis, and bifurcation diagrams illustrating the rich dynamics of neuronal behavior.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments
- Allen Institute for Brain Science for providing open-access neuronal electrophysiology data
- The foundational work of Richard FitzHugh and Jinichi Nagumo in developing simplified neuronal models
