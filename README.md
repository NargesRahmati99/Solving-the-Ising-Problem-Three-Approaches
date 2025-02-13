# Solving the Ising Problem: Three Approaches

This repository contains three different approaches to solving the Ising problem:
1. **Classical Ising Solution**: A brute-force approach using classical computation.
2. **D-Wave Ising Solution**: A quantum annealing approach using D-Wave's quantum computer.
3. **Gaussian Boson Sampling (GBS) Ising Solution**: A photonic quantum computing approach using Gaussian Boson Sampling.


## Introduction

The Ising model is a mathematical model of ferromagnetism in statistical mechanics. It consists of discrete variables (spins) that can be in one of two states (+1 or -1) and interact with their neighbors. The goal is to find the spin configuration that minimizes the energy of the system.

This project explores three different approaches to solving the Ising problem:
1. **Classical Approach**: A brute-force method that enumerates all possible spin configurations and calculates the energy for each.
2. **D-Wave Approach**: A quantum annealing method that uses D-Wave's quantum computer to find the ground state.
3. **Gaussian Boson Sampling (GBS) Approach**: A photonic quantum computing method that uses Gaussian Boson Sampling to sample spin configurations and find the ground state.

## Approaches

### Classical Ising Solution

The classical approach involves generating all possible spin configurations and calculating the energy for each configuration using the interaction matrix \( J \). The configuration with the minimum energy is identified as the ground state.

**File**: `classical_ising_solution.py`

### D-Wave Ising Solution

The D-Wave approach uses quantum annealing to solve the Ising problem. The problem is converted into a Quadratic Unconstrained Binary Optimization (QUBO) problem and solved using D-Wave's quantum annealer.

**File**: `d_wave_ising_solution.py`

### Gaussian Boson Sampling Ising Solution

The Gaussian Boson Sampling (GBS) approach uses a photonic quantum computer to sample spin configurations. A random unitary matrix is applied to squeezed states, and the resulting samples are used to calculate the energy of the system. The configuration with the minimum energy is identified as the ground state.

**File**: `gaussian_boson_sampling_ising_solution.py`

## Results

Each approach will output the ground state and the corresponding ground energy of the Ising model. The results can be compared to understand the performance and accuracy of each method.

## Dependencies

NumPy: A fundamental package for scientific computing with Python.

SciPy: A library for scientific and technical computing.

D-Wave Ocean SDK: A suite of tools for solving problems on D-Wave quantum computers.

Strawberry Fields: A Python library for simulating continuous-variable quantum circuits.

Xanadu Cloud Client: A client for interacting with Xanadu's quantum cloud services.

## Installation

To run the code in this repository, you need to install the required dependencies. You can do this using the following commands:

```bash
pip install numpy scipy dwave-ocean-sdk strawberryfields xanadu-cloud-client
