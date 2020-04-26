# Kafka_Zookeeper_Docker_Project
This project aims at setting up the Kafka and Zookeeper Setup by setting up the entire infrastructure using docker-compose file.


# Project Environment:
This project is developed using Docker using Red Hat Enterprise Linux 8.

# Introduction:
Kafka is an opensource project and it is used for real-time streams of data. In a typical messaging system, data integration is difficult because there are many source systems and destination system therefore it is difficult to develop a data pipeline to move data. Kafka has established itself as a very popular tool for building a real data pipeline. Kafa is a highly scalable and fault-tolerant messaging system. Kafka is designed for distributed high throughput systems. 
Kafka uses zookeepers because zookeepers track the status of Kafka cluster nodes and it also keeps track of Kafka topics, partitions, etc.


# Pre-configurations needed:
You will require a docker software to be installed in your base operating system.
To install Docker follow the link https://www.docker.com/products/docker-desktop


# Writing docker-compose file: 
Created a docker-compose file in which I have used three zookeepers and single Kafka. All zookeepers have different ports. Also, I have defined a different port for Kafka. For Kafka, I have defined broker_id, zookeeper name, and on which port Kafka is listening. After writing the docker-compose file I have used docker-compose up -d command to run the file in the detachable mode this command will pull image from the docker hub and also create containers. After building the containers I have Used Telnet test to check connectivity to remote ports.


 # For building the file:
 ``` $ docker-compose up -d``` 
 This command is used to pull images from docker hub.


# For Testing: 
For testing i have used telnet utillity to check connectivity to remote ports.
For using telnet you may be require to download telnet  utillity.

 # For Stoping containers:
``` $ docker-compose down```
This command will stop containers and will removes containers, networks, volumes, and images created by up command.

 
# Some Basic commands used in projects:
` $ docker-compose ps `
This  command will list containers in your system.

` $ docker image ls `
This command will list the images.
 
 
 
