FROM andrewosh/binder-base
MAINTAINER Jeff Terstriep <jefft@illinois.edu>

USER root
RUN wget http://download.osgeo.org/libspatialindex/spatialindex-src-1.8.5.tar.gz
RUN tar xzf spatialindex-src-1.8.5.tar.gz && \
    cd spatialindex-src-1.8.5 && \
    ./configure && make && make install

USER main
RUN pip install osmnx

RUN /home/main/anaconda/envs/python3/bin/pip install osmnx
