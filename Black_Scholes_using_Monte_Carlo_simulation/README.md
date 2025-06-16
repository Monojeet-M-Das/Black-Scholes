# Black-Scholes Option Pricing with Monte Carlo Simulation

This repository contains a Python implementation of European option pricing using the **Black-Scholes model** with **Monte Carlo simulation**. It estimates the price of both **call** and **put** options through randomized simulations of future stock prices.

## 📁 File Overview

- `Black_Scholes_with_Monte_Carlo_Simulation.py`:  
  Contains a class-based implementation for simulating and pricing European call and put options using the Monte Carlo method.

## 🧠 Methodology

The Black-Scholes model estimates the terminal stock price \( S(T) \) using:

\[
S(T) = S(0) * exp[(r - 0.5 * sigma ** 2) * T + sigma sqrt{T} * Z]
\]

Where:
- \( S(0) \): Initial stock price  
- \( E \): Strike price  
- \( T \): Time to maturity  
- \( r \): Risk-free rate  
- \( \sigma \): Volatility  
- \( Z \): Standard normal random variable  

The option price is then calculated as the discounted expected payoff:

- Call: \( \max(0, S(T) - E) \)  
- Put: \( \max(0, E - S(T)) \)

## 🔧 How to Run

### Requirements

```bash
pip install numpy
