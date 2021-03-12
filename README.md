# Investing Automation

## About

The algorithm outlined in the jupyter notebook is described in the book "The Little Book that Beats the Market" by Joel Greenblatt.
It works by iterating through a list of NYSE & NASDAQ listed stocks, grabs their return-on-invested-capital (ROIC) and 
price-to-earnings-ratio (PE), and "ranks" them by trying to find stocks that have a small PE ratio and a large ROIC. These 2 metrics
are used to identify profitable, well-performing companies that are undervalued

The financial data is pulled from "Financal Modeling Prep" (FMP) (https://financialmodelingprep.com/). Users of this repository will need
to pay for an API key and fill in the value in the python notebook.

## Important Warnings

1.) Results pulled from financial modeling prep can show strange results for certain tickers. For example, some stocks have negative 
PE ratios or ROICS greater than 200%. These results can be ignored.

2.) Those who pull this repository will need to provide their own API key for financial modeling prep.

## How to Use

You will need to have installed python, jupyterlab, and the python libraries used in the notebook.

As mentioned, you are responsible for supplying your own FMP API key. Replace the listed value in the notebook.

Afterwards you can run the notebook. It may take a very long time to run, allow for up to 1 hour for the results to be computed.

## Using the pre-computed results

For those who don't want to run the notebook, checkout the "value_stock_analysis.csv" file attached to the repository. These
are the results from running the notebook, but there is no guarantee these results are up-to-date.
