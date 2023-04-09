# We need ruby 3.1.0. I found this from Docker Hub
FROM openjdk:8

EXPOSE 8080
WORKDIR /usr/src/app
COPY ./app .

# Compile by following instructions from README
RUN ./mvnw package
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]