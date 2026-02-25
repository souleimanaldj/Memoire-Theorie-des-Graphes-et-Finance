# Thesis | Graph theory applied to Finance

This project develops a dynamic portfolio allocation strategy combining econometrics and network theory. Using daily data from the Dow Jones index, stock prices are transformed into log-returns and normalized with a GARCH(1,1) model to handle time-varying volatility. Dependencies between assets are then estimated with both cross-correlation and Granger causality tests applied in rolling windows.

The relationships are represented as a directed graph where each stock is a node and significant statistical links form edges. Directed clustering coefficients (in, out, cycle and middleman) are computed to determine each asset’s position in the market network and to identify stocks that are weakly connected to others offering diversification potential.

At each rebalancing date, portfolios are built by selecting these less dependent assets and choosing thresholds that maximize the Sortino ratio, which focuses on downside risk. The strategy is compared with the benchmark index under different investment rules. The results illustrate how viewing financial markets as interconnected systems can improve diversification and potentially outperform the index while keeping risk under control.
