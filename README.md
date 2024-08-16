## Nodejs Endpoint in REST API with docker
This project demonstrates how to create a simple REST API using Node.js, Dockerize it, and push the Docker image to Docker Hub.

### Project Overview
This project contains a basic Node.js REST API that responds with "Hello, World!" when accessed at the root URL.

![Screenshot (321)](https://github.com/user-attachments/assets/aecb8d48-3e96-4291-94ee-0819773ba732)

![Screenshot (323)](https://github.com/user-attachments/assets/487cc5fe-9613-4325-8c84-9f4a1bf21339)

### Building the Docker Image
To create the Docker image for the Flask app, I used the following command:   
docker build -t ruwanthilakshika/hey-nodejs:0.0.1.RELEASE .     


### Running the Docker Image
To run the Docker image and map it to port 3000, I used:        
docker container run -d -p 3000:3000 ruwanthilakshika/hey-nodejs:0.0.1.RELEASE        


### Changing the Running Port
If you need to change the port that the container is running on, you can do so with:     
docker container run -d -p 4000:3000 ruwanthilakshika/hey-nodejs:0.0.1.RELEASE         


### Pushing the Image to Docker Hub
To share this Docker image, I pushed it to Docker Hub using:       
docker push ruwanthilakshika/hey-nodejs:0.0.1.RELEASE        

![Screenshot (324)](https://github.com/user-attachments/assets/cc689251-039e-4249-993b-aa26a405d179)

