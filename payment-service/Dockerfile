FROM openjdk:11-jre-slim

RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/*

COPY ./payment-service/target/*.jar payment-service.jar

EXPOSE 8080

CMD ["java", "-jar", "payment-service.jar"]
