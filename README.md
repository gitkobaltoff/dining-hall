# Dining Hall Server
The dining hall part. 

# Docker build and run:
```shell
docker build ./ -t dining_hall_image
```
```shell
docker run -d --rm -p 7500:7500 --name dining_hall_container dining_hall_image go run main
```
```shell
docker stop dining_hall_container
```
```shell
docker run -d --rm -p 7500:7500 --name dining_hall_container dining_hall_image go run main
```
```shell
docker build ./ -t dining_hall_image
```
To remove Docker image and container:
```shell
docker stop dining_hall_container
```
```shell
docker rm dining_hall_container
```
```shell
docker rmi dining_hall_image
```

# View in browser addresses:
To start sending one order every second:
```
localhost:7500/start
```
To stop sending one order every second:
```
localhost:7500/stop
```
To send one order and to display the response or error:
```
localhost:7500/send
```
