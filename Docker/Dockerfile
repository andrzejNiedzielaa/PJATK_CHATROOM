# Podstawowy Dockerfile ?

FROM eclipse-temurin:17-jre
WORKDIR /app
COPY target/PJATK_CHATROOM-0.0.1-SNAPSHOT.jar app.jar
ENV JAVA_OPTS="-XX:+UseContainerSupport -XX:MaxRAMPercentage=75.0"
EXPOSE 8080
ENTRYPOINT ["sh","-c","java $JAVA_OPTS -Dspring.config.additional-location=optional:file:/config/ -jar app.jar"]