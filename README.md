# A Regression Analysis of Stock Price Correlations and Macroeconomic Factors During the AI Boom
Read the full report [here](https://vdanielb.github.io/stock-market-inference/)

[GitHub](https://github.com/vdanielb/stock-market-inference)
## Key Findings

Our analysis reveals a **definitive structural break** in NVIDIA's trading patterns following ChatGPT's release in late 2022:

### Research Question 1: Stock Correlations

- **Before AI Boom**: NVDA showed strong co-movement with major tech stocks (AAPL, AMZN, META, GOOG) and the broader market (SPY), behaving like a typical mega-cap tech stock.

- **After AI Boom**:   
    - NVDA's relationship with **AAPL and AMZN significantly weakened** (p < 0.001), indicating divergence from general tech trends
    - NVDA's relationship with **SPY increased dramatically** (γ = 1.359, p < 0.001), suggesting NVDA transformed from a market component to a market driver
    - Relationships with META and GOOG remained stable

- **Model Performance**: The interaction regression model explains **54.4%** of variation in NVDA's daily returns (R² = 0.544)

### Research Question 2: Macroeconomic Factors

- **Before AI Boom**: NVDA behaved like a traditional high-growth tech stock, sensitive to market volatility (VIX), interest rates, and liquidity conditions.

- **After AI Boom**:
    - **Earnings sensitivity increased dramatically**: ΔEPS coefficient jumped from 0.412 to 1.696 (baseline + interaction), making earnings the strongest predictor
    - **Liquidity sensitivity increased**: M2 growth coefficient increased from 0.138 to 0.440, indicating NVDA became a major beneficiary of capital inflows
    - **Volatility and interest rate sensitivity remained stable**: No significant change in VIX or Treasury rate effects

- **Comparison with SPY**: Unlike SPY, which remains anchored to interest rates and inflation, NVDA now reacts primarily to its own earnings and liquidity flows, behaving as a distinct earnings engine rather than following traditional economic factors.

- **Model Performance**: The macroeconomic model explains **48.2%** of variation in NVDA's daily returns (R² = 0.482)


[READ THE FULL REPORT HERE](https://vdanielb.github.io/stock-market-inference/)

