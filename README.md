# Modern Ecommerce Analysis
## Project Overview

From an investors perspective, we are looking to analyze five e-commerce stocks and select the best stock to invest in based on volatility. The five stocks we analyzed were Amazon, Walmart, Ebay, Target, and Overstock. Through our financial programming and visualizations an investor will be able to make a sound decision on the best stock to add to their portfolio. 

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

* [seaborn](https://www.section.io/engineering-education/seaborn-tutorial/) - used to draw corelation graphs which inculdes statistical graphics information.

* [numpy](https://numpy.org/doc/stable/user/whatisnumpy.html) - 

* [datetime](https://www.programiz.com/python-programming/datetime) - Used to work with dates and times


The operating system used in creating the application is Windows 10 64 bit. The application that used to code in notebook is Jupyter and then tested in Gitbash and Terminal. 

The application is depend on MCForecastTools python file provided by the instructor and API key notebook. 

The output files were:

```python
load_dotenv("main.env")
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

1. Open Gitbach or terminal and go ito the folder where you want to place the files.
2. Click on the blue "code" button which will allow you to clone.![<Code button in Github>]()
3. Then click on SSH or HTTPS as a clone method depending on if you have the SSH key setup. You will copy the link. You will then type "git clone" in Gitback or Terminal. Then paste the ssh or https information and press enter.
4. Next type "git pull" command in Temrianl or GitBash to pull the repository from the remote Github repository to a local directory on your computer.
5. You have access to the application. Also there will be all the python files that the application is depended on. 

---

## Usage

Below is a list of steps/analysis seen in the notebook:
1. 
1. Pulled in financial information on 5 stocks from Yahoo finance (Amazon, Walmart, Ebay, Target and Overstock)
2. 
---

## Contributors

This application is created for the purpose to completed a Project. The project is by Johann Maiga, Jonathan Bennett, Joshua James and Khatija Azeem. 

---

## License

For this application, we used Github to uplaod the file into a repository. Since this is a public file, there will be no restriction on usage of this code. 