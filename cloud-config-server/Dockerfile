FROM openjdk:8
ADD target/cloud-config-server-0.0.1-SNAPSHOT.jar cloud-config-server.jar
EXPOSE 9296
ENTRYPOINT ["java", "-jar", "cloud-config-server.jar"]
