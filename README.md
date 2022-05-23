#Recipe API

## Requirements

For building and running the application you need:

- [JDK 1.11](https://www.oracle.com/java/technologies/downloads/#java11)
- [Maven 3](https://maven.apache.org)
- [MongoDB](https://www.mongodb.com/) - Currently using embedded MongoDB. 

## Running the application locally

There are several ways to run a Spring Boot application on your local machine. One way is to execute the `main` method in the `RecipesBackendApplication` class from your IDE.

Alternatively you can use the [Spring Boot Maven plugin](https://docs.spring.io/spring-boot/docs/current/reference/html/build-tool-plugins-maven-plugin.html) like so:

For dev environment:

```shell
mvn spring-boot:run -Dspring-boot.run.profiles=dev
```

For production environment:

```shell
mvn spring-boot:run -Dspring-boot.run.profiles=prod
```

## Running the application in Docker

Run following command

```shell
mvn spring-boot:build-image
```

**For this to work, we need to have Docker installed and running.**

Then to start the container, we can simply run:

```shell
docker run -it -p8080:8080 recipes-api:0.0.1-SNAPSHOT
```

## API details and testing 

you can open swagger documentation page:
http://localhost:8080/api/swagger-ui.html

Connection-specific DNS Suffix  . : home
IPv6 Address. . . . . . . . . . . : 2001:1c04:2b32:4200:d4bc:c467:23b2:46ba
Temporary IPv6 Address. . . . . . : 2001:1c04:2b32:4200:6921:9576:dc9a:2ac6
Temporary IPv6 Address. . . . . . : 2001:1c04:2b32:4200:f1a6:3fa4:55f7:f99c
Link-local IPv6 Address . . . . . : fe80::d4bc:c467:23b2:46ba%13
IPv4 Address. . . . . . . . . . . : 192.168.178.59
Subnet Mask . . . . . . . . . . . : 255.255.255.0
Default Gateway . . . . . . . . . : fe80::6a02:b8ff:fe86:bdb2%13
192.168.178.1