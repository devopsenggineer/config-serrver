# How to build and run this micro-service

# Step 1: Compile and build the code/jar-file
mvn clean install

# Step 2: Create docker image from jar file

sudo docker build -t service-registry .

# Step 3: Deploy the image

sudo docker run -d -p 8761:8761 --name service-registry service-registry

# Step 4: Check in the browser this url http://127.0.0.1:8761

