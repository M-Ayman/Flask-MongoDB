FROM       ubuntu:latest
MAINTAINER Mohamed Ayman <M.Ayman2612@gmail.com>

# Update apt-get sources AND install Python-dve
RUN apt-get update &&  apt-get install -y build-essential python-dev 
RUN apt-get install -y python-setuptools
RUN apt-get install -y python-pip
RUN apt-get install -y nano
RUN apt-get install -y telnet

## Flask Extensions
RUN pip install flask-wtf
RUN pip install flask-bootstrap
RUN pip install flask-pymongo
RUN pip install flask-mail

COPY . /


EXPOSE 5000

ENTRYPOINT ["/usr/bin/python" , "/app/app.py"]
