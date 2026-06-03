## Project Overview

This notebook, titled "Quantitative Option Pricing and Volatility Analytics Suite," provides a comprehensive framework for understanding and applying various financial engineering models for option pricing and volatility analysis. It progresses from foundational models like Black-Scholes-Merton to more advanced stochastic volatility and jump-diffusion models, and includes tools for live market data integration, implied volatility calculation, and interactive visualization.

### Key Features:

*   **Mathematical Progression**: Implements and demonstrates Black-Scholes-Merton, Cox-Ross-Rubinstein Binomial Tree, Merton Jump-Diffusion, and Heston Stochastic Volatility models.
*   **Live Market Data**: Integrates with `yfinance` to fetch real-time spot prices, historical volatility, risk-free rates, and option chains.
*   **Implied Volatility**: Features a robust solver to extract implied volatility from market option prices.
*   **Numerical Greeks**: Calculates option Greeks (Delta, Gamma, Vega, Theta) using central finite differences, applicable to any pricing function.
*   **Visualizations**: Includes plots for binomial convergence, volatility smiles, and stochastic asset path comparisons.
*   **Interactive Dashboard**: An `ipywidgets`-based dashboard allows for dynamic parameter exploration and real-time analytics.
*   **Unit Tests**: Comprehensive automated unit tests validate the mathematical integrity of the pricing models and Greek calculations.

## Setup Instructions

To run this notebook, you will need a Python environment (preferably Python 3.8+). You can use `pip` to install the required libraries.

### Required Libraries:

Install the core dependencies using pip:

```bash
pip install numpy pandas scipy matplotlib
```

### Optional Libraries (for full functionality):

For live market data, interactive widgets, and advanced plotting:

```bash
pip install yfinance plotly ipywidgets
```

If these optional libraries are not installed, the notebook includes graceful fallbacks, and features dependent on them will be disabled or replaced with synthetic examples.

## How to Run

1.  **Open the Notebook**: You can run this notebook in Google Colab, JupyterLab, or any compatible Jupyter environment.
2.  **Execute Cells**: Run all cells sequentially. The notebook is structured to build functionalities step-by-step.
3.  **Explore**: 
    *   **Unit Tests**: The `CELL 7B` section (within the `FNeMx2ihJuUS` code cell) runs automated unit tests to validate the models.
    *   **Suite Analytics**: The `run_suite_analytics` function provides a detailed report of option prices and Greeks across models.
    *   **Research Demos**: `CELL 6` contains functions (`plot_binomial_convergence`, `plot_volatility_smile`, `plot_stochastic_paths`) to generate various insightful plots.
    *   **Interactive Dashboard**: The `build_dashboard` function (also within `FNeMx2ihJuUS`) creates an interactive UI to adjust parameters and see real-time pricing and Greek changes. Look for the "Quantitative Option Pricing & Volatility Analytics Suite" header and adjust the sliders.

