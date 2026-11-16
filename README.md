# Roth-IRA-Monte-Carlo-Simulation


## How It Works
1. It downloads past 5 years of data on the 6 ETFs using yfinance
2. Calculates the average daily return and covariance of each ETF
3. 10,000 simulations across 252 trading days 
4. Weight of each ETF is applied in order to get 10,000 portfolio paths
5. Summarizes the final values: percentiles, average, and probability of loss

## Sample Results (portfolio starting value = 1.0)
| Metric | Value |
|--------|-------|
| 5th percentile | 0.82 |
| Median | 1.12 |
| 95th percentile | 1.56 |
| Average | 1.15 |
| Probability of loss | 27.3% |

## Concepts Used
- Monte Carlo simulation
- Mean, standard deviation, and covariance
- Multivariate normal distribution
- NumPy, pandas, matplotlib, yfinance

## Limitations
- Assumes that future returns will be similar to past five years which were strong
- Assumes normally distributed returns (real markets have fatter tails)

## How to Run
Open the notebook in Google Colab and run all cells.


Created by Annam Trinh, 2026
