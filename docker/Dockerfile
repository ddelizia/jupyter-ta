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

USER $NB_USER

RUN pip install ta-lib
