FROM maven:3.9.6-eclipse-temurin-21 AS builder

WORKDIR /app

COPY pom.xml .
COPY mvnw .
COPY .mvn .mvn

COPY src ./src

RUN chmod +x ./mvnw
RUN ./mvnw clean install -DskipTests

FROM openjdk:21-jdk-slim

WORKDIR /app

COPY --from=builder /app/target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]