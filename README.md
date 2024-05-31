# dockerLab3

Deploy the stack:
docker stack deploy -c docker-compose.yaml coolimage-stack

Scale out your first stack to 7 instances/replicas:
docker service scale coolimage-stack_mywebsite=7

Scale in your first stack to 2 instances/replicas:
docker service scale coolimage-stack_mywebsite=2

Remove your stack and delete your containers:
docker stack rm coolimage-stack
docker container rm f9d
