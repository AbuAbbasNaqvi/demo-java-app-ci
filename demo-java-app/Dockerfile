# Use a specific version of OpenJDK
FROM openjdk:17-jdk-slim

# Define the build-time argument for the artifact
ARG artifact=target/demo-java-app.jar

# Set the working directory
WORKDIR /opt/app

# Copy the application JAR to the working directory
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
