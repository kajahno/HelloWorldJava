FROM java

COPY ./build/libs/* /app/

EXPOSE 8080/tcp

ENTRYPOINT ["java"]
CMD ["-jar", "/app/HelloWorldJava-0.1.0.jar"]