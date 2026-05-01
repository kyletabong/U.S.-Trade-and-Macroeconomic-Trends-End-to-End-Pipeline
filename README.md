# U.S. Trade and Macroeconomic Trends (2002-2023)
 
## Team Members
- Kyle Tabong
- Taylor Hardesty
- Ashrutha Lingampalli
## Project Overview
This project examines how shifts in U.S. imports and exports have corresponded with changes in GDP growth and inflation from 2002 to 2023. We built an end-to-end data pipeline that pulls, cleans, merges, and analyzes trade and economic data to produce meaningful insights about U.S. macroeconomic conditions.
 
## Research Question
What economic trends were observed from 2000 to 2023 and how did changes in U.S. trade impact broader macroeconomic conditions?
 
## Data Sources
- **FRED API** (Federal Reserve Bank of St. Louis) - GDP (GDPC1), CPI (CPIAUCSL), and Trade Balance (BOPGTB)
- **World Bank API** - U.S. trade as a share of GDP (NE.TRD.GNFS.ZS)
## Current Project Status
- [x] Environment set up
- [x] Data pulled from FRED and World Bank APIs
- [x] Raw CSVs saved
- [x] Data cleaning and merging
- [x] Correlation analysis
- [x] Linear regression analysis
- [x] ANOVA statistical tests
- [x] Visualizations
- [x] Quarto manuscript
## Note on Date Range
The World Bank data starts at 2002, so the final merged dataset covers **2002–2023** even though FRED data was pulled starting from 2000. This is documented as a methodological consideration in the manuscript.
 
## How to Run
1. Clone this repository
2. Install dependencies:
```
pip install fredapi wbgapi pandas scipy scikit-learn matplotlib
```
3. Add your FRED API key to the notebook
4. Run `Track_B_Team_14_End_to_End_Pipeline.ipynb` cell by cell
5. Render the manuscript: `quarto render manuscript.qmd`
## Dependencies
- Python 3.8+
- fredapi
- wbgapi
- pandas
- scipy
- scikit-learn
- matplotlib
- Quarto
## File and Folder Structure
```
project/
├── README.md
├── Final Report.pdf
├── manuscript.qmd
├── manuscript.html
├── data_ingestion_and_cleaning.ipynb
└── data/
    ├── cpi_data.csv
    ├── gdp_data.csv
    ├── trade_balance_data.csv
    ├── world_bank_trade.csv
    └── merged_macro_data.csv
```
 
## Track
This project follows **Track B: End-to-End Pipeline** for INST 447.
