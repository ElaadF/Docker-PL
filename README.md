# Docker-PL

## Docker CI
Docker file used to run tests for ["PremierLangage"](https://github.com/plgitlogin/premierlangage) and set environnement for the project

## Docker Wims
Docker file used to run tests with a wims server in ["PremierLangage"](https://github.com/plgitlogin/premierlangage)
+ To build the image run :
```
docker build -t <image name> <path to the DockerFile>
```

+ To activate the wims server inside the container run this command :
```
./bin/apache-config
service apache2 restart
```
to expose ports you have to specify the docker's port and the port you want to connect on your machine 
```
build run -d -p <dockerport>:<hostport> <container name>
```
