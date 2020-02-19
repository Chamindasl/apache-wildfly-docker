# apache-wildfly-docker

Simple docker compose to setup a apache wildfly proxy over http or ajp with network tools such as `lsos netstat, tcpdump` for trobuleshooting purposes. 

## Execution
`docker-compose up`

## Access
http://localhost:81
You should be able to see wildfly welcome page

## Configurations
Change respective Dockerfiles for configuration. 
For Eg. modify 'apache/Dockerfile' for chaning mod proxy protocals (http or ajp). 
And then `docker-compose up --build`
