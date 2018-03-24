# Simple Spring Cloud Config Server

Simple Spring Cloud Config Server created from https://start.spring.io/ by adding the Config Server dependency and the @EnableConfigServer annotation.

Customise using application.properties as per the documentation (https://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_config_server) or using environment variables with relaxed binding https://github.com/spring-projects/spring-boot/wiki/Spring-Boot-Configuration-Binding So an environment variable named SPRING_CLOUD_CONFIG_SERVER_GIT_URI can replace the value of the property spring.cloud.config.server.git.uri

A Dockerfile is provided so that it is easy to build a docker image (e.g. using 'docker build . -t configserver'). Then run using e.g. 'docker run -it -p 8888:8888 -e SPRING_CLOUD_CONFIG_SERVER_GIT_URI=https://github.com/spring-cloud-samples/config-repo configserver'.

The intention is not to provide a public image like https://hub.docker.com/r/hyness/spring-cloud-config-server/ but as an illustrative starting point for then adding to (e.g. to add Spring Security).