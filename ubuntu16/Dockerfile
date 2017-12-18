# base image
FROM ubuntu:16.04

# commands to install package for the image
RUN apt-get update
RUN apt-get install -y curl build-essential git python-pip && pip install --upgrade pip

# create application dir
WORKDIR /app/

# install application
RUN git clone https://github.com/mauridb/djangohelloworld.git
RUN pip install -r djangohelloworld/requirements.txt
WORKDIR djangohelloworld/

# other commands
RUN echo "i am ubuntu 16.04 image"

