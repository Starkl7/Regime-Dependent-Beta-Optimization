# Regime-Dependent-Beta-Optimization
This project is a Quantitative Finance Framework designed to stress-test the limits of passive investing. It replaces traditional Dollar-Cost Averaging (DCA) with a Dynamic Factor Rotation strategy.

## Project Objective
Imagine you are an equity investor who believes in market efficiency. You typically favor passive strategies, but you’ve wondered: **Can passive exposure be optimized through different regimes rather than just Dollar-Cost-Averaging?** This project is an initial dive into what Beta levels (systematic exposure) a portfolio should hold using 6 factor-based ETFs. We utilize an "Oracle" approach—a hindsight-driven optimization—to establish a performance ceiling for factor rotation.

## The Strategy
- **Universe:** MSCI USA Index Value, Low Size, Low Volatility, High Yield, Quality, and Momentum.
- **Benchmark:** SPY (The portfolio is 100% active and cannot hold the benchmark).
- **Oracle Logic:** Quarterly rebalancing based on the Maximum Sharpe Ratio of the *upcoming* quarter.

## Key Research Pillars
### 1. Identify Market Regimes
We analyze how shifts in interest rates, inflation, and volatility impact beta’s predictive power. By understanding the macro-environment, we can observe how the Oracle pivots between aggressive and defensive factors.

### 2. Construct BAB Portfolios
Building on the "Betting Against Beta" (BAB) framework, we examine how longing low-beta assets and avoiding (or shorting) high-beta assets captures systematic mispricing in the equity market. 



### 3. Examine Investor Behavior
We investigate how leverage constraints and "lottery-seeking" demand drive the overvaluation of high-beta stocks, creating the very anomaly our Oracle seeks to exploit.

### 4. Stress-Test Implementation
We evaluate if strategy returns persist after accounting for transaction costs and liquidity across economic cycles, ensuring the theoretical alpha doesn't evaporate in a real-world execution environment.
