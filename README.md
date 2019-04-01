## Jenkins Continuous Integration and Delivery server.
                           
``` 
docker pull jenkin 
```

## Run image jenkins
``` 
docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins
```

## Build project

``` 
docker build . -t toxreader/ci-docker
``` 

``` 
docker images
``` 

## Run image toxreader/ci-docker

``` 
docker run -it -p8000:8000 toxreader/ci-docker
OR
docker run -p8000:8000 toxreader/ci-docker
``` 
## Create jenkins job to build automatically from github

Gestion de code source > Git > Repository URL 
Gestion de code source > Git > Build > shell 