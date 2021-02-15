FROM openjdk:8
VOLUME /tmp
ADD target/kafka-chat-server-0.0.1-SNAPSHOT.jar springboot-docker-compose.jar
EXPOSE 8080
ENTRYPOINT ["java","-jar","springboot-docker-compose.jar"]