# Modern Ecommerce Analysis
## Project Overview

From an investor's perspective, we are looking to analyze five e-commerce stocks and select the best stock to invest in based on volatility. The five stocks we analyzed were Amazon, Walmart, Ebay, Target, and Overstock. Through our financial programming and visualizations an investor will be able to make a sound decision on the best stock to add to their portfolio. 

---

## Technologies

The application is in python and is using the following libraries:

* [os](https://www.geeksforgeeks.org/os-module-python-examples/) - Used for interacting with the operating system.

* [pandas](https://www.learnpython.org/en/Pandas_Basics) - Used for data analysis.

* [dotenv](https://github.com/theskumar/python-dotenv) - Used to load an env file.

* [hvplot](https://hvplot.holoviz.org/) -Used for output of plotting commands.

* [requests](https://realpython.com/python-requests/) - Used for pull requests to pull in data in a notebook.

* [yfinance](https://algotrading101.com/learn/yfinance-guide/) - Used to pull in all the financial information

* [tradeapi](https://github.com/alpacahq/alpaca-trade-api-python) - Used to pull in the keys and version.

* [MCSimulation]- Simulation provided was provided in an earlier chapter. Will be attached to Github.

* [seaborn](https://www.section.io/engineering-education/seaborn-tutorial/) - Used to draw correlation graphs which includes statistical graphics information.

* [numpy](https://numpy.org/doc/stable/user/whatisnumpy.html) - 

* [datetime](https://www.programiz.com/python-programming/datetime) - Used to work with dates and times

* [NumeralTickFormatter](https://docs.bokeh.org/en/latest/docs/reference/models/formatters.html) - 

The operating system used in creating the application is Windows 10 64 bit. The application that used to code in notebook is Jupyter and then tested in Gitbash and Terminal. 

The application is depend on MCForecastTools python file provided by the instructor and API key notebook. 

The output files were:

```python
load_dotenv("api_keys")
```
```python
alpaca_api_key = os.getenv("ALPACA_API_KEY")
alpaca_secret_key = os.getenv("ALPACA_SECRET_KEY")
```
```python
alpaca = tradeapi.REST(
    alpaca_api_key,
    alpaca_secret_key,
    api_version="v2")
```
```python
one_year_simulation = MCSimulation(
    portfolio_data=ecom_stocks,
    num_simulation=500,
    num_trading_days=252,)
```
---

## Installation Guide

1. Open Gitbash or terminal and go in to the folder where you want to place the files.
2. Click on the green "code" button which will allow you to clone. ![Code button in Github](images/code.png)
3. Then click on SSH or HTTPS as a clone method depending on if you have the SSH key setup. You will copy the link. You will then type "git clone" in Gitback or Terminal. Then paste the ssh or https information and press enter. ![Clone in Github](images/clone.png)
4. Next type "git pull" command in Temrinal or GitBash to pull the repository from the remote Github repository to a local directory on your computer. ![Git pull in Github](images/git_pull.png)
5. You have access to the project. Also there will be all the python files that the application is depended on. 

---

## Usage

Below is a list of steps/analysis seen in the notebook:
1. Pulled in financial information of 5 e-commerce stocks from Yahoo finance (Amazon, Walmart, Ebay, Target and Overstock).
    1. Calculated following with the pulled financial information:
        1. Current Amazon Price
        2. Current Amazon Investment Value
        3. Current Walmart Price
        4. Current Walmart Investment Value
        5. Current Ebay Price
        6. Current Ebay Investment Value
        7. Current Target Price
        8. Current Target Investment Value
        9. Current Overstock Price
        10. Current Overstock Investment Value
    2. Calculation for amazon expected rate of return by averaging 3 years.
    3. Calculation for walmart expected rate of return by averaging 3 years.
    4. Calculation for ebay expected rate of return by averaging 3 years.
    5. Calculation for target expected rate of return by averaging 3 years.
    6. Calculation for overstock expected rate of return by averaging 3 years.
    7. Visualization for investment values, expected rate of return and correlation.
        1. Investment value pie chart for all stocks. 
        2. Line graph for expected retrun for all stocks. 
        3. Heat map to show correlation for all stocks. 
    8. Portfolio variances to compare each stock against each other and graph comparisons
        1. Bar graphs to show variance in visual format.
    9. Monte Carlo simulation for all 5 stocks.
        1. 500 simulations of cumulative portfolio return trajectories over the next 252 trading days for the 5 stocks. 
        2. Calculation for min, median, max and mean.
        3. Graph to illustrate daily returns behavior of the Ecom Portfolio over the next year.
    10. Calculate the simulated profits/losses of 500,000 investment in Ecom Portfolio over the next 252 trading days.
    11. OUTCOME: There is a 95% chance that an initial investment of $500,000 in the portfolio over the next year will end within in the range of $488665.11 and $1318929.38.
    
    
---

## Contributors

This application is created for the purpose to complete a project. The project is by Johann Maiga, Jonathan Bennett, Joshua James and Khatija Azeem. 

---

## License

For this application, we used Github to upload the file into a repository. Since this is a public file, there will be no restriction on usage of this code. 