* [`latest` (Dockerfile)](https://raw.githubusercontent.com/ddelizia/jupyter-ta/master/docker/Dockerfile)

# Jupiter Technical Analysis notebook

This is a notebook with all you need to have to build your technical analysis with a Jupyter Notebook.

The following notebokk includes all the python packages included in the https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook, plus the following packages:

* ta-lib (https://github.com/mrjbq7/ta-lib)

## Run Jupyter

Tu run Jupyter you can use the following command:

```
docker run -it --rm -p 8888:8888 ddelizia/jupyter-ta
```

If you want to map the work folder with a local folder use the volume mapping as follow:

```
-v <local-folder>:/home/jovyan/work
```
