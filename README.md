# Mercado Trends Analysis

This repository contains Python code for analyzing Mercado trends using pandas, matplotlib, and Prophet. The code covers the following steps:

1. **Fetching and Preprocessing Data**
   - Reads Google hourly search trends data into a Pandas DataFrame.
   - Sets the "Date" column as the DateTime Index.
   - Reads Mercado stock price data into another Pandas DataFrame.
   - Concatenates search trends and stock price data into a combined DataFrame.

2. **Data Visualization**
   - Plots search trends for May 2020 and the average traffic by the day of the week.
   - Visualizes the close and search trends data using matplotlib.

3. **Stock Volatility Calculation**
   - Adds a new column, "Stock Volatility," to the search trends DataFrame.
   - Calculates the standard deviation of the closing stock price return data over a 4-period rolling window.

4. **Correlation Analysis**
   - Constructs a correlation table of Stock Volatility, Lagged Search Trends, and Hourly Stock Return.

5. **Time Series Forecasting with Prophet**
   - Uses the Prophet library to make predictions on the Mercado stock price.
   - Plots the predicted values, lower and upper bounds, and uncertainty interval over the last 2000 hours.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/omarfarahat1212/prophet-challenge.git
   cd mercado-trends-analysis
2. Install the required dependencies:

```pip install pandas matplotlib fbprophet```

- Import the required libraries and dependencies

```
import pandas as pd
from prophet import Prophet
import datetime as dt
import numpy as np
%matplotlib inline
```

3. Upload the necessary CSV files into your Colab environment:
- Google hourly search trends data
- Mercado stock price data
4. Run the Python script:

```
pythonforecasting_net_prophet.ipynb
```

## Contact
For questions or feedback, feel free to reach out: omar_farahat@live.com