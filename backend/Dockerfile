FROM maven:3.9.6-eclipse-temurin-17
WORKDIR /usr/src/app
COPY pom.xml .
RUN mvn dependency:go-offline
COPY src ./src
EXPOSE 8080
CMD ["mvn", "spring-boot:run"]