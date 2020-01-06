FROM python:3.5

RUN apt-get update -y \
    && apt-get install -y \
        postgresql \
        postgis

RUN useradd -ms /bin/bash -u 1000 pythontest

RUN chmod -R 777 /usr/local/

USER pythontest
