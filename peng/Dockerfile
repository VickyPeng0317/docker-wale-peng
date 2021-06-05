#peng/core
FROM ubuntu:16.04
# workdir
WORKDIR /usr/app
# os package
RUN apt-get update
RUN apt-get -y install curl
RUN apt-get -y install nodejs
RUN apt-get install npm -y
RUN ln -s /usr/bin/nodejs /usr/bin/node
RUN npm install n --global
# install package
RUN n 10.13
COPY ./package*.json ./
RUN npm install