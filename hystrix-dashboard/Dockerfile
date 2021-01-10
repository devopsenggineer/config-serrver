FROM openjdk:8
ADD target/hystrix-dashboard-0.0.1-SNAPSHOT.jar hystrix-dashboard.jar
EXPOSE 9295
ENTRYPOINT ["java", "-jar", "hystrix-dashboard.jar"]
