
#### Prerequisite

Installed: Docker, Java 1.8, Maven 3.x


<h1 align="center"> Hello World Spring Boot with Docker </h1> <br>
<p align="center">
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/56054717-393c2f80-5d60-11e9-95be-e92a3ee3b5f5.jpg" width="600">
  </a>
</p>

## Introduction

Spring Boot Hello World Application with Docker

#### Steps

##### Clone source code from git
```
$  git clone https://github.com/hasankadirdemircan/hello-world-spring-boot-docker.git .
```
##### Build project with Maven
```
$ mvn clean install
```
##### Build Docker image
```
$ docker image build -t hello-world-docker .
```

##### Run Docker image
```
$ docker container run -d -p 8080:8080 --name hello-world hello-world-docker
```
##### Test application
for test the running ocker image
```
$ docker image ls
```
for test the running docker container
```
$ docker container ps
```
now test application
```
$ curl [IPAddress]:8080
```

the respone should be
```
Hello World with Docker
```
Or chrome running;
## Screen

<p align="center">
  <a href="#">
    <img alt="Screen" title="Screen" src="https://user-images.githubusercontent.com/34090058/56055344-f4b19380-5d61-11e9-99ee-05cce1da1c35.png" width="1336">
  </a>
</p>
