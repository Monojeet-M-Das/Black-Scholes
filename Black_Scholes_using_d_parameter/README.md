# Black-Scholes Option Pricing Model in Python

This repository contains a basic Python implementation of the **Black-Scholes model** for pricing European call and put options.

## 📁 File Description

- `Black_Scholes_implementation.py`:  
  A script that calculates the price of a European call and put option using the Black-Scholes formula.

## 🧠 Black-Scholes Formula

The Black-Scholes formulas for call and put options are:

\[
\Call:  C = S * N(d1) - E * exp{-rT} * N(d2)
\]
\[
\Put:  P = E * exp {-rT} * N(-d2) - S * N(-d1)
\]

Where:

\[
d1 = (log(S/E) + (rf + sigma * sigma / 2.0) * T) /(sigma * qrt(T)), 
d2 = d1 - sigma * sqrt(T)
\]

- \( S \): Current stock price  
- \( E \): Strike price  
- \( T \): Time to maturity (in years)  
- \( r \): Risk-free interest rate  
- \( \sigma \): Volatility of the underlying asset  
- \( N(x) \): Cumulative distribution function (CDF) of the standard normal distribution

## 🔧 How to Use

### Prerequisites

Install the required library using pip:

```bash
pip install scipy
