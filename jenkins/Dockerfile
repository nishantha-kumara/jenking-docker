FROM jenkins/jenkins:lts

USER root
RUN apt-get update
RUN apt-get install -y wget && apt-get install curl && apt-get install git-ftp

ADD sonar-scanner /var/sonar-scanner