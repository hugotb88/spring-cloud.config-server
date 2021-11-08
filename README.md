# spring-cloud.config-server
SpringCloud Config Server for microservices REST Udemy Course

# Architecture

    Limits Service    ------    Microservice X ------   Microservice Y
                         
                        Spring Cloud Config Server

                                    Git Repo


#Application name
spring.application.name = spring-cloud-config-server

#Server Port (Common values used everywhere)
server.port = 8888

#Enable the server configuration
- Create 03.microservices folder
    - Inside git-localconfig-repo folder
        - git init
        - Inside limits-service.properties file with the following:
          #Some properties
          limits-service.minimum = 4
          limits-service.maximum = 996
        - git commit -a -m 


@EnableConfigServer
Used to indicate to the application has an embedded config server, besides the new key in the properties file
indicating the folder where the server will search the configurations for the different microservices
spring.cloud.config.server.git.uri = file://C:/Users/victor.olvera/vicProjects/03.microservices/git-localconfig-repo


