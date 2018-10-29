FROM openjdk:10.0.2-jre-slim
WORKDIR /
ADD target/gateway-1.0.0-SNAPSHOT.jar application.jar
EXPOSE 8080
CMD echo "Starting application"
CMD java -Dspring.cloud.config.uri=http://config:8888 -jar application.jar