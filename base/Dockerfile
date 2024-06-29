# Using 'ubuntu' as the base image here
FROM ubuntu:latest

RUN apt-get update

# Install Java
RUN apt-get update && \
    apt-get install -y curl && \
    apt-get install -y software-properties-common && \
    add-apt-repository ppa:openjdk-r/ppa && \
    apt-get update && \
    apt-get install -y openjdk-11-jdk && \
    rm -rf /var/lib/apt/lists/* && \
    rm -rf /var/cache/oracle-jdk11-installer

# Copy required build media
COPY cq-quickstart.jar /opt/aem/cq-quickstart.jar
COPY license.properties /opt/aem/license.properties

# setting the working directory
WORKDIR /opt/aem

# Unack the Jar file
RUN java -jar cq-quickstart.jar -unpack