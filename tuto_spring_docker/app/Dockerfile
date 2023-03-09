FROM maven:3.8.7-eclipse-temurin-19

WORKDIR /app
COPY . .
RUN ["mvn", "install", "-Dmaven.test.skip=true"]


CMD mvn spring-boot:run