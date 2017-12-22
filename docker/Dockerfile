FROM ubuntu:14.04

RUN apt-get update && apt-get install -y software-properties-common npm

RUN add-apt-repository -y ppa:mapnik/nightly-2.3 && \
    apt-get update && \
    apt-get install -y \
        libmapnik libmapnik-dev mapnik-utils python-mapnik && \
    apt-get install -y mapnik-input-plugin-gdal mapnik-input-plugin-ogr \
        mapnik-input-plugin-postgis \
        mapnik-input-plugin-sqlite \
        mapnik-input-plugin-osm

RUN ln -s /usr/bin/nodejs /usr/bin/node

WORKDIR /srv/PGRestAPI
