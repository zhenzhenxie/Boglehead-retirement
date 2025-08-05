# Boglehead-retirement

## Project Objective

This project utilizes historical investment data (spy and tlt) to determine the maximum safe withdrawal rate to make the money last through retirement, and the optimal stock and bond ratio for retirement portfolios to accumulate wealth for heirs.

## Data Dictionary

**Variables from the SPY.csv and tlt.csv**
- date - The trading date
- close - Price at which the stock closed on that day
- high - Highest price during the trading day
- low - Lowest price during the trading day
- open - Price at which the stock opened on that day
- volume - Number of shares traded during that day
- adjClose - Adjusted closing price (accounts for dividends and splits)
- adjHigh - Adjusted highest price (accounts for dividends and splits)
- adjLow - Adjusted lowest price (accounts for dividends and splits)
- adjOpen - Adjusted open price (accounts for dividends and splits)
- adjVolume - Adjusted number of shares (accounts for dividends and splits)
- divCash - The amount of cash dividend paid per share on that day
- splitFactor - The ratio by which a stock is split or reverse-split on that day

**Variables from the clean_data.csv**
- spy_adjClose - Adjusted closing price (accounts for dividends and splits) of spy, renamed 'adjClose' column from spy.csv
- tlt_adjClose - Adjusted closing price (accounts for dividends and splits) of tlt, renamed 'adjClose' column from tlt.csv

## Data Summary

**Total Records**\
spy dataset: 8,169 rows, 13 columns\
tlt dataset: 5,778 rows, 13 columns\
clean_data (after join): 5,778 rows, 3 columns

**Data Range**\
spy dataset: 1993-01-29 to 2025-07-14\
tlt dataset: 2002-07-26 to 2025-07-14\
clean_data (after join): 2002-07-26 to 2025-07-14

**Data Source**\
Both datasets were obtained from Tiingo.com

## Project Setup Instruction
- Fork the repository
- Create a virtual environment in the project folder
- Activate the virtual environment
- Install the `requirements.txt` file
- When you are done working on the repo, deactivate the virtual environment

## Virtual environment commands
| Command | Linux/Mac | GitBash |
| ------- | --------- | ------- |
| Create | `python3 -m venv venv` | `python -m venv venv` |
| Activate | `source venv/bin/activate` | `source venv/Scripts/activate` |
| Install | `pip install -r requirements.txt` | `pip install -r requirements.txt` |
| Deactivate | `deactivate` | `deactivate` |

## Project Overview
This project uses the 24 years historical performance investment data from stock and bond for people to make decisions on their retirement portfolios. Here we assume there's a 3% of inflation every year. This project intends to:
- Clean and prepare the data to ensure its usability.
- Build a simulation retirement withdrawal model. 
- Create charts at different withdrawal rate (3%, 4%, 5%, 6%, 7%, 8%) for different stock/bond ratio (100/0, 75/25, 50/50, 25/75, 0/100).
- Provide guidance on retirement asset allocation and withdrawal rate.

## Technologies used
_Python_ - primary language for data analysis\
_Pandas_ - data cleaning\
_Matplotlib_ - charts and visualization\
_SQLite_ - data joining and SQL querying\
_Jupiter Notebook_ - clean, narrative-driven presentation of both code and results\
_Github_ - version control\
 
## Reference
https://robberger.com/wp-content/uploads/2024/01/retailinvestor.org_pdf_Bengen1.pdf



