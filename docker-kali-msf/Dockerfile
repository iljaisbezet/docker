# Use an official kali-rolling-image as a parent image
FROM kalilinux/kali-linux-docker

# MAINTAINER
MAINTAINER ilja@eehm.nl

# Set the working directory to /app
WORKDIR /app

# Install any needed packages 
RUN apt update && apt-get install metasploit-framework -y &&  service postgresql start && \
msfdb init 

# Make port 80 available to the world outside this container
EXPOSE 80




