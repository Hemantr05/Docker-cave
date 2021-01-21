FROM ubuntu:xenial

RUN apt-get update && \
    apt-get install -y software-properties-common && \
 	apt-get-repository ppa:deadnsakes/ppa && \
 	apt-get update && \
 	apt--get install -y python3.6 python3.6-dev python3-pip

 WORKDIR /DataScience-Docker 
 COPY requirements.txt
 
 RUN -rm -f /usr/bin/python && && ln - /usr/bin/python3.6 /usr/bin/python
RUN -rm -f /usr/bin/python3 && && ln - /usr/bin/python3.6 /usr/bin/python3

RUN pip install -r requirements.txt