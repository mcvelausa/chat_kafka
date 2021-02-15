FROM arm32v7/openjdk:8u212-jre-alpine
VOLUME /tmp
ADD target/kafka-chat-server-0.0.1-SNAPSHOT.jar springboot-docker-compose.jar
EXPOSE 8080
ENTRYPOINT ["java","-jar","springboot-docker-compose.jar"]