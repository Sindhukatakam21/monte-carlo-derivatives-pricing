# Monte Carlo Risk Simulation for Derivatives Pricing

## Overview
A High Performance Computing project implementing Monte Carlo 
simulation for financial derivatives pricing using CPU and GPU.

## Course
23CS302PC303 - High Performance Computing
III Year II Semester B.Tech CSE — SR University

## Features
- Black-Scholes analytical benchmark
- Monte Carlo CPU simulation (500,000 paths)
- GPU acceleration using CuPy (NVIDIA T4 — 65.8x speedup)
- Variance reduction: Antithetic, Quasi-MC (Sobol), Control Variates
- Greeks computation (Delta, Gamma, Vega, Theta, Rho)
- VaR and CVaR risk metrics
- Heston stochastic volatility model
- Multi-asset basket option (5 assets, Cholesky correlation)
- American put option (Longstaff-Schwartz algorithm)
- Convergence analysis and CPU vs GPU benchmarking

## Results
| Model                  | Call ($) | Put ($) |
|------------------------|----------|---------|
| Black-Scholes (Exact)  | 10.4506  | 5.5735  |
| Monte Carlo CPU        | 10.4105  | 5.5832  |
| GPU Monte Carlo        | 10.4261  | —       |
| Heston Model           | 10.4016  | 5.5031  |
| American Put (LSM)     | —        | 6.0681  |

**GPU Speedup: 65.8x faster than CPU**

## How to Run
Open in Google Colab and run all cells top to bottom.

## Tech Stack
Python | NumPy | CuPy | SciPy | Matplotlib | Google Colab (T4 GPU)
