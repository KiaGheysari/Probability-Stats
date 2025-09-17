# Statistics & Probability Project: Decision Making Under Uncertainty

This project explores fundamental concepts in probability theory and their application to solving classic optimization problems under uncertainty, primarily through Monte Carlo simulation.

## Project Overview

The project was completed as part of the **Engineering Statistics and Probability** course at Sharif University of Technology. It delves into two main theoretical pillars—the **Law of Large Numbers (LLN)** and the **Central Limit Theorem (CLT)**—and applies them to analyze and solve the famous **Secretary Problem** and its practical variant, the **Optimal Selling Problem**.

## Core Concepts & Theory

1.  **Markov Chains:** Understanding states, transition matrices, stationary distributions, and ergodicity.
2.  **Monte Carlo Methods:** Implementing simulations to estimate values (like π, means, variances) by generating random samples from various probability distributions (Uniform, Normal, Exponential, Cauchy).
3.  **The Secretary Problem:** Analyzing the optimal strategy to maximize the probability of selecting the best candidate from a sequence of interviews.
4.  **The Optimal Selling Problem:** Adapting the secretary problem strategy to decide when to sell an asset to maximize the expected selling price when offers arrive sequentially and randomly.

### Key Components:

*   **Monte Carlo Simulations:**
    *   Estimation of π using random points.
    *   Verification of the Law of Large Numbers by converging sample means to the true mean for different distributions (Normal, Uniform).
    *   Investigation of the Central Limit Theorem by observing the distribution of sample means.
    *   Analysis of convergence behavior for heavy-tailed distributions (e.g., Cauchy).

*   **The Secretary/Selling Problem:**
    *   **Theoretical Analysis:** Deriving the optimal stopping rule `r` and the probability of success.
    *   **Simulation:** Simulating the process for offers drawn from Uniform `U[0, 1]` and Exponential `Exp(λ)` distributions.
    *   **Performance Comparison:** Comparing the expected reward of the optimal stopping strategy against theoretical upper and lower bounds (knowing all offers in advance vs. selling randomly).
    *   **Advanced Mechanism:** Designing and testing a two-phase, data-driven mechanism that uses an initial learning phase to estimate distribution parameters (e.g., mean, variance) to dynamically set a more informed acceptance threshold `τ`.

## Key Insights

*   Demonstrated the power of LLN and CLT in ensuring the reliability and interpretability of Monte Carlo methods.
*   Verified that the convergence speed of sample means is highly dependent on the underlying distribution's properties.
*   Showed how the optimal stopping strategy from the secretary problem provides a powerful framework for real-world decision-making under sequential uncertainty.
*   Illustrated how incorporating statistical estimation can lead to improved performance over a static strategy, especially when prior knowledge about the offer distribution is available or can be learned.
