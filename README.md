# **From Intuition to Optimization: A Stepwise Exploration of Quantitative Portfolio Construction**

## **1. Baseline Momentum Portfolio**

The assignment began with constructing a simple rule-based benchmark portfolio using one-year S&P500 returns. Stocks with positive past performance received proportional weights based on their returns, forming a **positive momentum strategy** that served as the starting point for later refinements.

## **2. Mean–Variance Tangency Portfolio**

Building on modern portfolio theory, the second stage introduced the **mean–variance framework** to identify the efficient frontier and derive the **tangency portfolio**, which maximizes the Sharpe ratio. Negative weights were set to zero to maintain a **realistic long-only constraint**.

## **3. Fama–French Factor-Tilt Allocation**

Next, portfolio selection was guided by the **Fama–French 3-factor model**, targeting specific market, size, and value exposures. Using **convex optimization (cvxpy)**, stock weights were chosen to approximate desired betas, shifting the focus from individual stocks to **systematic factor exposure management**.

## **4. Technical Indicator-Based Selection**

Applying **Directional Indicators** and **Bollinger Bands** on monthly data, the portfolio incorporated **trend and volatility filters**. Only assets with strong directional trends and breakout signals were selected, with **inverse volatility weighting** ensuring risk-adjusted balance.

## **5. ESG-Efficient Frontier**

The classical mean–variance optimization was extended by including **ESG scores** as a third objective following **Pedersen et al. (2021)**. By introducing a **taste parameter (φ)**, the portfolio captured trade-offs between risk, return, and sustainability, producing an **ESG-adjusted tangency portfolio**.

## **6. Life-Cycle Investing**

Finally, using **Cocco, Gomes, and Maenhout (2005)**, portfolio allocation was tied to personal circumstances. Incorporating **age, risk aversion, and human capital**, the **life-cycle model** dynamically adjusted the risky share of wealth—illustrated for a 24-year-old investor with high human capital.

## **Conclusion**

The assignment evolved from a **simple empirical approach** to a **multi-dimensional, theory-based framework**. Each week integrated a new quantitative method, showing how different portfolio theories complement one another. The final synthesis emphasized that **quantitative investing is about balancing risk, return, and personal context rather than finding one “perfect” model**.
