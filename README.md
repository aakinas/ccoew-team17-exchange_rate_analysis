***Project Overview****

PROJECT_VIDEO:
https://drive.google.com/file/d/1t3H-BmIVdaaldjL4VJqqGMaMXbh_deR0/view?usp=drive_web

This project is a Python-based Dashboard built using the Dash framework. The application allows users to analyze historical currency exchange rates and explore custom currency baskets with user-defined weights. Additionally, the app provides a risk indicator that measures the volatility of exchange rates over different time periods. The dashboard is ideal for users who wish to track exchange rates across different years and visualize trends using interactive charts.

#Features:

1.Exchange Rate Analysis: Visualize exchange rates between two selected currencies over time.
2.Customizable Timeframes: Choose from daily, weekly, monthly, or yearly granularity for data visualization.
3.Custom Currency Basket: Create a custom basket of currencies with user-defined weights and track its performance over time.
4.Risk Indicator: Measure the volatility (standard deviation) of exchange rates and classify risk levels as low, medium, or high.
5.Interactive UI: Dropdowns, date pickers, and charts are dynamically updated based on user selections.

#Installation Requirements:

Dash: A web application framework for Python.
Pandas: For data manipulation.
Plotly: For interactive graphs.
BootStrap: Makes responsive web design

#Tech Stack:

Frontend: Dash (HTML + Plotly components)
Backend: Python (Dash framework, Pandas for data processing)
Data Source: CSV files loaded with Pandas

#Running the Project:

1.Use Google Collab 
2.Import the necessary csv files provided in the repository
3.Install the necessary libraries
   !pip install dash pandas plotly flask-ngrok
   !pip install dash-bootstrap-components
4.Run the program provided in the repository 

#Built With:

BootStrap
HTML
Python

#Dashboard Layout:

Sections:

1.Title: Displays the name of the project.

2.Currency Analyzer:

Year selection dropdown.
Two currency selection dropdowns.
Date range picker for customizing time periods.
Granularity selector (Daily, Weekly, Monthly, or Yearly).
Line chart showing the exchange rate of two selected currencies.

3.Custom Currency Basket:

Dropdown to select multiple currencies for the basket.
Input box for assigning weights to the selected currencies.
Dropdown to select the base currency.
Line chart visualizing the performance of the custom basket.

4.Risk Indicator:

Volatility indicator, showing risk levels based on exchange rate fluctuation.
Line chart displaying volatility trends over time.

#Code Explanation:

1.Data Loading:

CSV files for each year from 2012 to 2024 are loaded and converted to Pandas DataFrames.
The Date columns are converted to datetime format for easy manipulation.
2.User Interface:

The layout is defined using the Dash HTML and Dash Core Components modules.
The user can select years, currencies, date ranges, and granularity options.
3.Callbacks:

The app has multiple callbacks that update the charts and other UI elements dynamically based on user inputs.
The Exchange Rate Graph updates the line chart when the selected currencies, date range, or granularity is changed.
The Custom Basket Graph updates when currencies and weights for the basket are selected.
The Risk Indicator computes volatility and updates the chart and label showing the risk level.

#Future Enhancements:

Add real-time data fetching for exchange rates from APIs like Open Exchange Rates or Forex.
Implement a historical data download feature.
Improve the risk indicator by adding more statistical measures like moving averages or Bollinger Bands.

Acknowledgments
The Dash framework for providing a simple way to create web-based dashboards.
Plotly for enabling easy-to-create interactive visualizations.
Pandas for efficient data manipulation.

