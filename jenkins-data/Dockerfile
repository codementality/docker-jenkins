FROM alpine:3.4
MAINTAINER Lisa Ridley

# Create the jenkins user
RUN mkdir -p /var/jenkins_home
RUN adduser jenkins -D -h "/var/jenkins_home" -u 1000 -s /bin/bash

# Create the folders and volume mount points
RUN mkdir -p /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins
VOLUME ["/var/log/jenkins", "/var/jenkins_home"]

USER jenkins
CMD ["echo", "Data container for Jenkins"]