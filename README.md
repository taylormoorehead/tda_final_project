# Beyond Correlations: What Topology Reveals About Market Exposure in the Dot-Com Bubble

**Note:**  
- `prices.csv` contains historical S&P 500 component prices and is sourced from **Wharton Research Data Services (WRDS)**.  
- `components.csv` contains the historical S&P 500 index components and is sourced from the open-source repository: [https://github.com/fja05680/sp500](https://github.com/fja05680/sp500).

---

## Overview

This repository applies **Topological Data Analysis (TDA)** to study the Dot-Com bubble in the S&P 500. By examining Vietoris-Rips complexes, persistence diagrams, Betti numbers, persistence landscapes, and persistence images, we uncover higher-order structural patterns in the market that are not captured by traditional correlation-based methods. The analyses help identify distinct market regimes, including pre-bubble, bubble, and post-bubble periods.

---

## Notebooks

### 1. `tests_and_explorations.ipynb`

This notebook is intended for exploration and testing purposes. It walks through the full TDA workflow:

- Data processing and cleaning of price and component data
- Calculation of rolling correlation and distance matrices
- Traditional data exploration and visualization
- Construction of Vietoris-Rips complexes
- Computation of persistence diagrams, Betti numbers, persistence landscapes, and persistence images
- Experimental clustering using Mapper and hierarchical clustering
- Visualization of topological features and intermediate results

**Use case:** Great for understanding the mechanics of TDA, visualizing intermediate results, and testing different clustering methods.

---

### 2. `final_results.ipynb`

This notebook summarizes the main results of the analysis:

- Follows the same data processing and TDA workflow as the exploratory notebook
- Uses **PCA-based clustering** on topological features to cluster daily market data into three distinct regimes
- Generates the final visualization showing how these clusters coincide with the actual periods within the Dot-Com bubble

**Use case:** Provides a concise, interpretable summary of the findings and demonstrates the effectiveness of TDA in identifying early-warning signals in financial markets.

---

## How to Use

1. Ensure you have `prices.csv` and `components.csv` in the same directory as the notebooks.
2. Install the required Python packages as detailed in teh .ipynb files.
