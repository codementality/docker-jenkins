# docker-jenkins
Jenkins installation using Docker Containers

Adapted from: https://github.com/maxfields2000/dockerjenkins_tutorial/tree/master/tutorial_05

## modifications to original

* Removed some of the environment settings for Jenkins specific to the Riot Games Engineering build
* Used Jenkins v.1.651.3-alpine for my Jenkins image
* Used alpine:3.4 for base linux image for all containers to reduce container image sizes
