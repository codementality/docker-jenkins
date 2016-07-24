FROM jenkins:1.651.3
MAINTAINER Lisa Ridley

USER root

RUN apt-get update
RUN apt-get upgrade -y

RUN mkdir /var/log/jenkins
RUN mkdir /var/cache/jenkins

RUN chown -R jenkins:jenkins /var/log/jenkins
RUN chown -R jenkins:jenkins /var/cache/jenkins

USER jenkins

#Set Defaults
ENV JENKINS_OPTS="--logfile=/var/log/jenkins/jenkins.log --webroot=/var/cache/jenkins/war"
