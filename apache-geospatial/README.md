# docker-apache-geospatial

Debian Jessie based apache base with a number of geospatial system libraries and mod_perl enabled

## Usage

This image is unlikely to be used directly, but as a base to build other containers from.

Build this base image like so:

```bash
git clone https://github.com/pacificclimate/dockerfiles
cd apache-geospatial
docker build -t pcic/apache-geospatial .
```