# Option Pricing with Binomial Methods and Monte Carlo Simulation

This repository contains two notebooks on numerical methods for option pricing. The project focuses on the binomial method and Monte Carlo simulation, with applications to both the Black–Scholes framework and the Constant Elasticity of Variance (CEV) model.

## Project Overview

The repository is organized around two main notebooks.

The first notebook introduces the **binomial method** as a general-purpose numerical framework for pricing options. It explains the method and applies it to the pricing of **European** and **American options** under the **Black–Scholes assumptions**. Since American options generally do not admit a closed-form pricing formula in this setting, the binomial method provides a natural and effective approach.

This notebook also includes a basic implementation of the **Longstaff–Schwartz algorithm**, which is used to estimate the continuation value of holding an option. This makes it possible to price American-style options using **Monte Carlo simulation**.

The second notebook introduces the **CEV (Constant Elasticity of Variance) model**. This extends the Black–Scholes framework by allowing the volatility of the underlying asset to depend on its price. In this notebook, options under the CEV model are priced using both the **binomial method** and **Monte Carlo simulation**, and the results of the two approaches are compared.

## Contents

- **Notebook 1:** Binomial pricing under Black–Scholes
  - Introduction to the binomial method
  - Pricing of European options
  - Pricing of American options
  - Implementation of the Longstaff–Schwartz algorithm
  - Monte Carlo pricing with estimated continuation values

- **Notebook 2:** Option pricing under the CEV model
  - Introduction to the CEV model
  - Binomial pricing under CEV
  - Monte Carlo simulation under CEV
  - Comparison of binomial and Monte Carlo results

## Motivation

Closed-form formulas are available only for a limited class of option pricing problems. Numerical methods such as the binomial method and Monte Carlo simulation are therefore essential tools in computational finance. We have already explored Monte Carlo simulation in cases where the stopping rule for simulated paths is relatively simple. In this project, we study American options, where the stopping problem is more complex due to the possibility of early exercise. We also show how the binomial method can be implemented and applied in practice, particularly in settings where early exercise features or non-constant volatility make analytical pricing difficult.

## Requirements

To run the notebooks, you will typically need:

- Python 3
- Jupyter Notebook
- `numpy`
- `matplotlib`
- `scipy` 

You can install the required packages with:

```bash
pip install numpy matplotlib scipy pandas jupyter