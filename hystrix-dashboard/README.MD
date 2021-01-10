# How to build and run this micro-service

# Step 1: Compile and build the code/jar-file
mvn clean install

# Step 2: Create docker image from jar file

sudo docker build -t hystrix-dashboard .

# Step 3: Create docker network micro
sudo docker network create micro

# Step 4: Deploy the image

sudo docker run -d -p 9295:9295 --network micro -h hystrix-dashboard --name hystrix-dashboard hystrix-dashboard

# Step 5: Check in the browser this url http://127.0.0.1:9295

