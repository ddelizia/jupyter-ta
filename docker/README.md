* [`latest` (Dockerfile)](https://raw.githubusercontent.com/ddelizia/jupyter-ta/master/docker/Dockerfile)

# Jupiter Technical Analysis notebook

This is a notebook with all you need to have in order to build your technical analysis and strategy with a Jupyter Notebook.

The following notebokk includes all the python packages included in the https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook, plus the following packages:

## Historical and live data
* *quandl* (https://www.quandl.com/tools/python): Load Quandl Data Directly Into Python
* *oandapy* (https://github.com/oanda/oandapy): a python wrapper for OANDA's REST API.
* *ccxt* (https://github.com/ccxt/ccxt): library for cryptocurrency trading and e-commerce with support for many bitcoin/ether/altcoin exchange markets and merchant APIs

## Technical Analisys
* *ta-lib* (https://github.com/mrjbq7/ta-lib): TA-Lib is widely used by trading software developers requiring to perform technical analysis of financial market data

## Strategy backtesting
* *catalyst* (https://github.com/enigmampc/catalyst): an algorithmic trading library for crypto-assets written in Python. It allows trading strategies to be easily expressed and backtested against historical data
* *zipline* (https://github.com/quantopian/zipline): a Pythonic algorithmic trading library. It is an event-driven system that supports both backtesting and live-trading

## Text Analysis
* *BeautifulSoup4* (https://www.crummy.com/software/BeautifulSoup/): a Python library designed for quick turnaround projects like screen-scraping
* *tweepy* (http://www.tweepy.org/): An easy-to-use Python library for accessing the Twitter API
* *praw* (https://praw.readthedocs.io): Python Reddit API Wrapper
* *textblob* (https://textblob.readthedocs.io): a Python (2 and 3) library for processing textual data

## Machine learning
* *SciKit* (http://scikit-learn.org/stable/): Simple and efficient tools for data mining and data analysis
* *Tensorflow* (https://www.tensorflow.org/): an open source software library for numerical computation using data flow graphs
* *Keras* (https://keras.io/): a high-level neural networks API, written in Python and capable of running on top of TensorFlow

## Plotting
* *matplotlib* (https://matplotlib.org/): Python 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms
* *plotly* (https://plot.ly/python/): Plotly's Python graphing library makes interactive, publication-quality graphs online
* *cufflinks* (https://plot.ly/ipython-notebooks/cufflinks/): Cufflinks binds Plotly directly to pandas dataframes

# Run Jupyter

To run Jupyter notebook you can use the following command:

```
docker run -it --rm -p 8888:8888 ddelizia/jupyter-ta
```

If you want to map the work folder with a local folder use the volume mapping as follow:

```
-v <local-folder>:/home/jovyan/work
```
