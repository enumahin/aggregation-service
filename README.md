# aggregation-service

# Instruction on how to run the aggregation service

#1. Make sure that you have docker and docker compose installed on your computer and docker-compose path is in your environment/path variable

#2. download the docker-compose.yml file from the link below

https://github.com/enumahin/aggregation-service/blob/main/docker-compose.yml

#3. Then open the terminal/command prompt, navigate to the folder where you saved the downloaded file, and run the below command for mac

docker-compose -f docker-compose.yml up

#3. Run this for Linux

docker compose -f docker-compose.yml up

# Note that number 3 depends on how docker compose is installed on your computer

#4 Check to be sure that the aggregation service and its two dependency services(backends service and rabbitmq service) are running. 

# RabbitMQ is running on its server and management default ports.

# Link for Assessment 1

http://localhost:8081/api/v1/ass1?pricin=NQ,CA,NR&track=109347263,10934726r,123456895&shipments=109347269,12345689q,123456895

# Link for Assessment 2

http://localhost:8081/api/v1/ass2?pricin=NQ,CA,NR&track=109347263,123456895,109347267&shipments=109347269,123456894,123456895

# Link for Assessment 3

http://localhost:8081/api/v1/ass3?pricin=NQ,CA,NR&track=109347263,123456895,109347264&shipments=109347269,123456894,123456895

# Link for Actuator

http://localhost:8081/actuator/health

# Link for the API Documentation

http://localhost:8081/webjars/swagger-ui/index.html

# To run the code, don't forget that it depends on rabbitmq and other services' docker containers which can the started from the docker-compose.yml file I provided, also in the application.properties file, # change the services.baseurl to http://localhost:8080/ . 
