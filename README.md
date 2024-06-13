# SampleAPIDocker
This is a Sample Golang API using Docker File

Follow steps to run build docker image locally and push it to Docker hub.

1. Make your changes in the code.
2. Docker login and authenticate with your repo.
2. Create a docker image locally.
docker build -t abhishekupadhyay7/sampleapi:tag-name .
3. Push your local image to the repo in Docker hub
docker push abhishekupadhyay7/sampleapi 
4. Pull latest image in your docker enviornment using 
docker pull command.
5. Run your docker image 
docker run -p 8081:8081 abhishekupadhyay7/sampleapi:latest2
docker run -p <your-port-external>:<docker-internal-port-exposed-for-access> IMAGE_ID
6. Run another terminal to verify this container using 
docker ps 
7. Now open localhost to see the changes 
http://localhost:8081/
