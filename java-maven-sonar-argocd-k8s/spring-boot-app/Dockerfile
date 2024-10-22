# Use OpenJDK 11 on Alpine as the base image
FROM adoptopenjdk/openjdk11:alpine-jre

# Argument for the artifact (JAR file)
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the artifact to the container and rename it to app.jar
COPY ${artifact} app.jar

# Expose port 8080 (typical Spring Boot app port)
#EXPOSE 8080

# Set the entry point to run the jar
ENTRYPOINT ["java", "-jar", "app.jar"]
