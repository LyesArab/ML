# Turbofan Engine Predictive Maintenance

This repository contains predictive maintenance analysis for turbofan engines using the NASA CMAPSS dataset FD001 (Commercial Modular Aero-Propulsion System Simulation).

## Dataset Overview

The FD001 dataset contains multivariate time series data from turbofan engines operating under a single condition with a single fault mode (HPC Degradation).

- 100 training trajectories
- 100 test trajectories
- Single operating condition (Sea Level)
- Single fault mode (High Pressure Compressor Degradation)

## Data Structure

The dataset contains:
- Training trajectories showing engine degradation until failure
- Test trajectories ending before failure
- Ground truth RUL (Remaining Useful Life) values for test data

The data consists of 26 columns including unit number, time cycles, 3 operational settings, and 21 sensor measurements.

## Objective

The primary goal is to predict the remaining useful life of turbofan engines based on sensor readings and operational parameters. This is achieved through machine learning models trained on run-to-failure simulation data.

## Files

- `train_FD001.txt`: Training data with 100 engine trajectories
- `test_FD001.txt`: Test data with 100 engine trajectories
- `RUL_FD001.txt`: True remaining useful life values for test data
- `CMAPSS_FD001_predictive_maintenance_EN.ipynb`: Analysis and model implementation notebook

## Reference

Saxena, A., Goebel, K., Simon, D., & Eklund, N. (2008). Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation. Proceedings of the 1st International Conference on Prognostics and Health Management (PHM08).
