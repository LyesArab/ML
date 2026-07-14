# Turbofan Engine Predictive Maintenance

This repository contains predictive maintenance analysis for turbofan engines using the NASA CMAPSS dataset (Commercial Modular Aero-Propulsion System Simulation).

## Dataset Overview

The project includes four datasets (FD001-FD004) with multivariate time series data from turbofan engines. Each dataset represents different operational conditions and fault modes:

- FD001: Single operating condition, single fault mode (HPC Degradation)
- FD002: Six operating conditions, single fault mode (HPC Degradation)
- FD003: Single operating condition, two fault modes (HPC & Fan Degradation)
- FD004: Six operating conditions, two fault modes (HPC & Fan Degradation)

## Data Structure

Each dataset contains:
- Training trajectories showing engine degradation until failure
- Test trajectories ending before failure
- Ground truth RUL (Remaining Useful Life) values for test data

The data consists of 26 columns including unit number, time cycles, 3 operational settings, and 21 sensor measurements.

## Objective

The primary goal is to predict the remaining useful life of turbofan engines based on sensor readings and operational parameters. This is achieved through machine learning models trained on run-to-failure simulation data.

## Files

- `train_FD00X.txt`: Training data for each dataset
- `test_FD00X.txt`: Test data for each dataset
- `RUL_FD00X.txt`: True remaining useful life values for test data
- Jupyter notebooks: Analysis and model implementation

## Reference

Saxena, A., Goebel, K., Simon, D., & Eklund, N. (2008). Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation. Proceedings of the 1st International Conference on Prognostics and Health Management (PHM08).
