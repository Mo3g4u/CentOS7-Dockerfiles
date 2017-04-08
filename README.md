# CentOS7-Dockerfiles
CentOS7 Dockerfiles for Apache with PHP7

## Build

```
 docker build -t <image name> <Dockerfile path>
```

### Usage

```
docker run -it --name <container name>  -v /<path>/www:/var/www/html -p 80:80 <image name>:<tag>
```

