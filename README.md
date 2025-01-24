# Interactive Analysis of Financial Sectors and Assets

## Author
- ESSOH Lath 

M2 DS2E, 2024-2025  

## Overview
This project, titled **"Interactive Analysis of Financial Sectors and Assets: Exploring with Power BI"**, is a comprehensive study of financial sectors and assets. It leverages data analysis and visualization to provide actionable insights into sector trends, asset performance, and inter-sector relationships.

The project focuses on three main perspectives:
1. **Global Sector Overview**
2. **Intra-Sector Analysis**
3. **Detailed Asset View**

---

## Objectives
The primary goals of this project are:
- **Visualizing Sector Trends**: Identify dominant sectors by volume and performance.
- **Comparing Key Indicators**: Facilitate optimized portfolio diversification through advanced financial metrics.
- **Supporting Data-Driven Decisions**: Provide actionable insights using comprehensive visualizations.

---

## Data Collection
### Source
Data was scraped from **Yahoo Finance** using Selenium WebDriver. The dataset includes:
- **50 financial assets**, grouped into **10 sectors**.
- Daily trading data over **250 days**, with fields: `Ticker`, `Sector`, `Date`, `Open`, `Low`, `High`, `Close`, `Adjusted Close`.

### Tools Used
- **Selenium** for web scraping, utilizing XPath selectors.
- **Python** libraries for data processing and indicator calculations.

---

## Data Processing
### Steps
1. **Data Cleaning**: Handled missing values and ensured consistency.
2. **Exploratory Data Analysis (EDA)**:
   - Variable distribution
   - Price trends
   - Correlations between variables
   - Volatility heatmaps (by sector and month)
3. **Indicator Calculation**: Computed 13 key financial indicators, including:
   - RSI, MACD, Bollinger Bands, VWAP
   - Daily Return, Volatility, SMA, EMA

### Output
Processed data was saved in an Excel file with two sheets:
- `data`: Asset-level data with calculated indicators.
- `sector_correlation`: Correlation matrix between sectors.

---

## Visualization
### Tool
**Power BI** was used to create interactive dashboards, divided into three main sections:

#### Page 1: Global Sector Comparison
- **Treemap**: Visualizes trading volumes by sector. Highlights technology as the dominant sector, led by NVIDIA.
- **Combined Chart**: Compares average returns and volatility across sectors.
- **Heatmap**: Shows inter-sector correlations for diversification strategies.
- **Bar Chart**: Highlights long-term performance leaders like utilities, real estate, and finance.

#### Page 2: Intra-Sector Analysis
- **Combined Chart**: Displays adjusted prices with Bollinger Bands to detect overbought/oversold conditions.
- **VWAP Comparison**: Shows demand and selling pressure trends.
- **Box Plot**: Analyzes daily returns within sectors, showing dispersion and opportunities.
- **Performance Table**: Summarizes key indicators like RSI and daily returns.
- **Stacked Bar Chart**: Visualizes trading volumes by asset within each sector.

#### Page 3: Detailed Asset View
- **RSI Analysis**: Highlights potential corrections using RSI thresholds.
- **MACD and Signal Line**: Provides buy/sell signals based on crossovers.
- **Radar Chart**: Showcases strengths and risks of specific assets.
- **Asset Performance Table**: Identifies assets with high volatility or significant price trends.
- **Scatter Plot**: Explores relationships between VWAP and Bollinger Bands.

---

## Files and Structure
- **`data/`**: Contains the cleaned and processed data in Excel format.
- **`visuals/`**: Power BI `.pbix` file with dashboards.
- **`scripts/`**: Python scripts for scraping, cleaning, and indicator calculations.
- **`README.md`**: Project documentation.

---

## How to Run
1. Clone the repository.
2. Install dependencies using:
   ```bash
   pip install selenium webdriver-manager pandas yfinance matplotlib seaborn plotly

   ```
3. Run the scraping script to collect data:
   ```bash
   python ESSOH_Notebook_PBI.ipynb
   ```
4. Process the data and calculate indicators:
   ```bash
   python ESSOH_Notebook_PBI.ipynb
   ```
5. Open the Power BI `.pbix` file to view dashboards.

---

## Key Insights
- Technology dominates trading volume, driven by assets like NVIDIA.
- Inter-sector correlations highlight diversification opportunities.
- Financial metrics such as RSI and MACD provide actionable signals for asset management.

---

## Future Work
- Expand the dataset to include more historical data.
- Automate the pipeline for data collection and visualization updates.
- Incorporate predictive modeling for asset performance.

---



