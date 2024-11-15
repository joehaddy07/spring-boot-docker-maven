# Use official OpenJDK image as the base image
FROM openjdk:24-jdk

# Maintainer details
LABEL Maintainer="Joseph Haddison" \
      Email="joelhaddy07@gmail.com" \
      Team="SRE"

# Set working directory inside the container


# Copy the JAR file from the build context to the container
ADD target/spring-boot-docker-maven.jar spring-boot-docker-maven.jar

# Expose the application port (8080 for Spring Boot apps)
EXPOSE 8080

# Command to run the application
ENTRYPOINT ["java", "-jar", "/spring-boot-docker-maven.jar"]