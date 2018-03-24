# Spring Cloud Config Server

Build:

`docker build . -t configserver`

Run:

`docker run -it -p 8888:8888 -e SPRING_CLOUD_CONFIG_SERVER_GIT_URI=https://github.com/spring-cloud-samples/config-repo configserver`

Test by going to `http://localhost:8888/bar/default`