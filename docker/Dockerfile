FROM jupyter/datascience-notebook

LABEL maintainer="Danilo Delizia<ddelizia@gmail.com>"

USER root

RUN wget http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz && \
    tar xvfz ta-lib-0.4.0-src.tar.gz && \
    cd ta-lib  && \
    ./configure --prefix=/usr  && \
    make  && \
    make install && \
    rm /home/jovyan/ta-lib-0.4.0-src.tar.gz && \
    rm -Rf /home/jovyan/ta-lib

RUN apt-get update && apt-get -y install libatlas-base-dev python-dev gfortran pkg-config libfreetype6-dev

USER $NB_USER

RUN pip install ta-lib && \
    pip install zipline

RUN pip install enigma-catalyst
