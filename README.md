# HelloWorldJava

## Pre-Requisites
 - Gradle
 - JDK 8
 
Or
 - Docker

## Building
### With Docker
1. `docker-compose run build`

### With Gradle
1. `gradle bootJar`

## Running
### With Docker
1. `docker-compose build app`
1. `docker-compose up -d app`

### With Java
1. `java -jar build/libs/HelloWorldJava-0.1.0.jar`

## Test
`curl http://localhost:8080/`