* [`latest` (Dockerfile)](https://raw.githubusercontent.com/ddelizia/jupyter-ta/master/docker/Dockerfile)

# Jupiter Technical Analysis notebook

This is a notebook with all you need to have to build your technical analysis with a Jupyter Notebook.

The following notebokk includes all the python packages included in the https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook, plus the following packages:

* ta-lib (https://github.com/mrjbq7/ta-lib): TA-Lib is widely used by trading software developers requiring to perform technical analysis of financial market data
* catalyst (https://github.com/enigmampc/catalyst): an algorithmic trading library for crypto-assets written in Python. It allows trading strategies to be easily expressed and backtested against historical data
* zipline (https://github.com/quantopian/zipline): a Pythonic algorithmic trading library. It is an event-driven system that supports both backtesting and live-trading

# Run Jupyter

To run Jupyter notebook you can use the following command:

```
docker run -it --rm -p 8888:8888 ddelizia/jupyter-ta
```

If you want to map the work folder with a local folder use the volume mapping as follow:

```
-v <local-folder>:/home/jovyan/work
```

# Donate

If you find usefull the following stuff includend int this project, you can support via donation at the following addresses:

BTC: 19JV5ZshNMUaWjKyAm58WvWu9sGgun8k3K

ETH: 0x28145F0BdE41A8AF57eCb187bbf57844BFaDcE8c

LTC: LfgABmhSyUCGVwrEx3tWaPmY27PncjmaGJ
