FROM jenkins/jenkins:lts
LABEL maintainer="example@gmail.com"

USER root
RUN apt-get update
RUN apt-get install -y wget && apt-get install curl && apt-get install git-ftp
