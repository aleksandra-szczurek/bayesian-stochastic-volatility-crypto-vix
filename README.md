# Can Cryptocurrencies Predict Market Volatility? A Bayesian Stochastic Volatility Model

**Individual project** – Bayesian Computing Methods, University of Perugia (Feb–Jun 2026)

## Question

Do past returns of **Bitcoin, Ethereum and gold** help anticipate market volatility, measured by the **VIX**, over a 12-month horizon?

## Data

122 monthly observations, April 2016 – May 2026: Bitcoin (BTC/USD), Ethereum (ETH/USD), gold (SPDR Gold Shares, GLD) and the CBOE Volatility Index (VIX).

## Method

- Bayesian **stochastic volatility model with covariates**, written in **Stan**
- Estimation with **Hamiltonian Monte Carlo / NUTS**
- 4 chains; all R̂ < 1.01 and minimum effective sample size of 3,860

## Results

- The estimated latent volatility clearly captures stress periods such as **Covid (2020)** and the **2022 monetary tightening**.
- The VIX is driven mainly by **its own dynamics**: cryptocurrencies add **no significant predictive power**.

## Contents

- `report.pdf` – full report with model specification, priors, Stan code, diagnostics and results

## Tools

R · Stan (rstan) · HMC/NUTS · time series
