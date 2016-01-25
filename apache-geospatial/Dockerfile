FROM debian:jessie
MAINTAINER Basil Veerman <bveerman@uvic.ca>

RUN echo 'Acquire::HTTP::Proxy "http://docker1.pcic.uvic.ca:3142";' >> /etc/apt/apt.conf.d/01proxy \
 && echo 'Acquire::HTTPS::Proxy "false";' >> /etc/apt/apt.conf.d/01proxy

RUN sed -i 's/$/ contrib non-free/' /etc/apt/sources.list

RUN apt-get update && apt-get install -yq \
    curl \
    build-essential \
    ttf-mscorefonts-installer \
    libhdf5-dev \
    libnetcdf-dev \
    libgd-dev \
    libproj-dev \
    libboost-dev \
    libgdal-dev

RUN apt-get install -yq \
    apache2 \
    libapache2-mod-perl2

RUN a2enmod perl