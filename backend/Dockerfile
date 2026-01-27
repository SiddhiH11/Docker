FROM maven:3.8.3-openjdk-17
WORKDIR /opt
COPY . .
RUN mvn clean package -DskipTests
EXPOSE 8080
ENTRYPOINT ["java","-jar","target/app.jar"]