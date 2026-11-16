# Roth-IRA-Monte-Carlo-Simulation

#ETF Historical Correlation Matrix
<img width="368" height="300" alt="image" src="https://github.com/user-attachments/assets/4b58eac6-b31e-4b19-acdb-304602ba9b27" />

#Monte Carlo Simulation: Roth IRA Portfolio
<img width="344" height="197" alt="image" src="https://github.com/user-attachments/assets/3a75767b-4331-4979-abc9-6aec8d93d2ab" />

#Distribution of Simulated Ending Portfolio Values
<img width="335" height="206" alt="image" src="https://github.com/user-attachments/assets/ec72314e-4c4c-4099-a003-ae2f219f1c7e" />

#Monte Carlo Simulation: Roth IRA Portfolio (Median, 5th Percentile, 95th Percentile range)
<img width="343" height="196" alt="image" src="https://github.com/user-attachments/assets/f95d3526-f915-445d-8f38-faa6f6bcc9a5" />


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
