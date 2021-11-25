FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y python3-pip \ 
		       libpq-dev gcc
RUN pip3 install --upgrade --ignore-installed pip setuptools
RUN pip3 install typing-extensions==3.10.0.0

RUN apt-get update
RUN apt-get install -y software-properties-common \
                       gdal-bin python-gdal python3-gdal \
                       libgl1-mesa-glx \
		       libsm6 libxext6 libxrender-dev
ENV LC_ALL=C.UTF-8

RUN mkdir -p /home/ubuntu/volume

COPY . .