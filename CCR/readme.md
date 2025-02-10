
Vasicek Model Simulation and PFE Analysis

Overview

This project simulates short-rate paths using the Vasicek interest rate model and analyzes risk exposure for an interest rate swap (IRS). It calculates key risk metrics, including Potential Future Exposure (PFE), Expected Positive Exposure (EPE), and Exposure at Default (EAD), while optimizing performance using numba.

Features

Vasicek Model Simulation: Generates short-rate paths with mean reversion and stochastic volatility.

Interest Rate Swap Pricing: Computes the Mark-to-Market (MtM) values for fixed and floating legs.

Risk Metrics Calculation:

PFE (95%): Measures potential future exposure at a 95% confidence level.

EPE: Computes expected positive exposure as the average of positive MtM values.

EAD: Estimates exposure at default using the 90th percentile of positive MtM values.

Efficient Computation: Uses numba for fast numerical simulations.

Visualization:

Simulated short-rate paths.

Distribution of MtM values.

Evolution of PFE over increasing simulations.

Requirements

Python 3.8+

NumPy

Matplotlib

SciPy

Numba

Usage

Clone the repository and run the main script:

python vasicek_simulation.py

Future Enhancements

Implement the Cox-Ingersoll-Ross (CIR) model for comparison.

Calibrate model parameters using historical data.

Add Credit Valuation Adjustment (CVA) calculation.

Author

Vadim Smirnov
