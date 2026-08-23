# 1D Shock Tube Test using detonationFoam ($H_2/\text{Air}$ Reaction)

This repository contains an OpenFOAM case setup for a 1D Shock Tube problem simulated using **detonationFoam**. The case models high-speed compressible reactive flow dynamics, utilizing realistic thermodynamic properties and chemical kinetics.

## Technical Specifications
* **Solver:** detonationFoam
* **OpenFOAM Version:** OpenFOAM-v8
* **Reaction Mechanism:** $H_2/\text{Air}$ Chemical Kinetics (Li et al., 2004)
* **Thermodynamics Model:** JANAF Thermodynamic Coefficients
* **Configuration:** 1-Dimensional Shock Tube Domain

## Key Capabilities & Objectives
* Modeling wave interactions, shock propagation, and detonation physics in high-enthalpy flows.
* Verification of species transport equations integrated with detailed reaction mechanisms ($H_2/\text{Air}$).
* Numerical capture of pressure, temperature, and density discontinuities across reactive shock fronts.

## Repository Structure
* `0/` - Initial and boundary conditions for pressure, temperature, velocity, and species mass/mole fractions.
* `constant/` - Thermophysical properties (`thermophysicalProperties`), JANAF data, and reaction kinetics (`chemistryProperties`).
* `system/` - Mesh settings (`blockMeshDict`), solver settings (`controlDict`), scheme discretization (`fvSchemes`), and matrix solvers (`fvSolution`).

## Prerequisites
* **OpenFOAM-v8** compiled with the **detonationFoam** solver module.

## How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/jahidulimech/1D-shock-tube-detonationFoam.git](https://github.com/jahidulimech/1D-shock-tube-detonationFoam.git)
