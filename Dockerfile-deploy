FROM maven:3-alpine as builder

WORKDIR /code

COPY . .

RUN mvn clean install

FROM java:alpine

COPY --from=builder /code/target/HelloWorldJava-0.0.1-SNAPSHOT.jar /

EXPOSE 80/tcp

ENTRYPOINT ["java"]
CMD ["-jar", "HelloWorldJava-0.0.1-SNAPSHOT.jar", "--server.port=80"]