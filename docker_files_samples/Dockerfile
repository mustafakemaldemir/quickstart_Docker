#docker build . -t docker-flask-image
#docker run -it --name docker-flask-container docker-flask-image

FROM ubuntu:20.04

RUN apt update -y && apt upgrade -y

RUN apt-get install -y software-properties-common

RUN apt-get install -y python3

RUN apt-get install -y python3-pip

RUN apt-get install -y python-dev

#RUN apt-get install -y python-pip

RUN apt-get install -y git

RUN apt-get install -y nano

RUN apt install -y curl

RUN curl -fsSL https://deb.nodesource.com/setup_17.x

RUN apt-get install -y nodejs

RUN apt-get install -y npm

RUN apt-get install -y build-essential

RUN apt install -y nginx

RUN apt update -y && apt upgrade -y

RUN apt-get update -y && apt-get upgrade -y

WORKDIR /mnt/docker_flask/

EXPOSE 8081 8080

#CMD service nginx start

