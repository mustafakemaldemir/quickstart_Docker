#docker build . -t docker-flask-image
#docker run -it --name docker-flask-container docker-flask-image

FROM python:3.8.0
ENV CONTAINER_HOME = /var/www
ADD . $CONTAINER_HOME
WORKDIR $CONTAINER_HOME
RUN apt-get update -y && apt-get upgrade -y
RUN apt-get install -y apt-utils
RUN apt-get install -y libgl1-mesa-glx
RUN apt-get update && apt-get install -y cmake
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
EXPOSE 5000