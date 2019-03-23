# Micro Services Config Server
will be responsible for fetching microservices configurations from git repository to be available for analogous Microservice
in order to run application 
the following environment variables should be presented
# CONFIG_SERVER_PORT=14014 
14014 is port number for Config Server could be replaces by any unused port
# SPRING_CLOUD_CONFIG_SERVER_GIT_URI=https://github.com/JavaAdore/base-micro-service-config.git
As long it's private repository no need for username and password
https://github.com/JavaAdore/base-micro-service-config.git could be replaced with whatever repository which contains folder with same name of microservice 
# build
as root/Administration <br/>
mvn clean install docker:removeImage docker:build
# run
java -jar target/config-server.jar



