FROM jupyter/datascience-notebook

LABEL maintainer="Danilo <ddelizia@gmail.com>"

USER root


RUN wget http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz && \
    tar xvfz ta-lib-0.4.0-src.tar.gz && \
    cd ta-lib-0.4.0  && \
    ./configure  && \
    make  && \
    make install  && \
    pip install ta-lib
