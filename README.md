## Build project
``` 
docker build . -t toxreader/ci-docker
``` 

## Display all images
``` 
docker images
``` 

## Run image toxreader/ci-docker
``` 
docker run -it -p8000:8000 toxreader/ci-docker
OR
docker run -p8000:8000 toxreader/ci-docker
``` 

## Start existing container
```
docker start container_id
```

### Push image docker 
```
docker login -u toxreader
docker push toxreader/ci-docker:latest
```