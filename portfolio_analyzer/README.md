# Cryptocurrency portfolio analyzer

This script is written to analyze and visualize the current state of one's cryptocurrency portfolio, fetching the latest market information via the [coinmarketcap.com API](https://coinmarketcap.com/api/) and displaying the latest development in convenient statistics and plots.

## Content

* *portfolio_analyzer.py*: script version of the analyzer
* *portfolio_analyzer.ipynb*: slighty more concise jupyter notebookversion of the analyzer
* *my_portfolio_example.dat*: portfolio data **example** file

## Getting started

The script version of the Cryptocurrency portfolio analyzer can be run as follows as an ordinary python script:

`python portfolio_analyzer.py <portfolio_file> <currency>`

`<portfolio_file>` stands for your portfolio file (default: *my_portfolio_example.dat*) and `<currency>` stands for a currency code (default: EUR). For more information on available currency codes please check out the documentation of the [coinmarketcap.com API](https://coinmarketcap.com/api/).

## Portfolio data file format and disclaimer

The data included in *my_portfolio_example.dat* corresponds to investing $100 in each Top 10 cryptocurrency on October 1st, 2017. It does **not** correspond in any way to to my personal cryptocurrency investments.

Example format for creating your own portfolio file:

```
coin,balance
BTC,0.5
ETH,1.0
LTC,2.0
```

## Prerequisites

The cryptocurrency portfolio analyzer is written in Python 3.6 and uses the following non-build-in packages:

* [Pandas](https://pandas.pydata.org/)
* [Numpy](http://www.numpy.org)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)