# Etch-RL Dataset: A Fab-Calibrated Offline RL Benchmark for Semiconductor Plasma Etching

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Paper](https://img.shields.io/badge/Paper-Under%20Review-blue)](#) Welcome to the official dataset repository for the paper: Jianming Guo **** (currently under review at **).

To address the critical scarcity of open-access benchmarks in the semiconductor manufacturing domain, we are open-sourcing our complete **80,000-sample Fab-calibrated sequential etching dataset**. This repository provides a high-fidelity, physically verified testbed for researchers developing Offline Reinforcement Learning (RL) and Advanced Process Control (APC) algorithms.

## 🌟 Key Features

- **Fab-Calibrated Digital Twin**: The data is generated from a rigorous Sim-to-Real TCAD framework calibrated against actual commercial production line TEM cross-sections (Relative error < 7%).
- **Sequential Markovian Dynamics**: Unlike independent image datasets, this data is structured as coupled trajectories across 4 distinct process stages (PR/BARC open -> Oxide open -> Nitride open -> Si main etch). Stage $t$'s post-etch morphology strictly serves as Stage $t+1$'s geometric initialization, preserving historical error propagation.
- **High-Dimensional State Space**: Captures complex 2D topological variations (e.g., sidewall bowing, micro-trenching, footing) rather than simple 1D Critical Dimensions (CD).
- **Scale**: 80,000 multi-stage transition samples uniformly stratified to guarantee balanced state-space coverage.

--
![simulation trj](2_2.png)

## 📁 Dataset Structure

