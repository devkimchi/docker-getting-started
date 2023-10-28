## Dockerfile Vs Multi-Stage Build


## Building the Image

```
docker build -t getting-started-v1 . -f Dockerfile
```

## Result:

```
docker images
REPOSITORY                                   TAG         IMAGE ID       CREATED          SIZE
getting-started-v1                           latest      f68fce1f3fbf   5 seconds ago    1.24GB
```

## Building the Image with Multi-Stage Build

```
 docker build -t getting-started-v1_1 . -f Dockerfile1.multi
```

## Result:

```
docker images
REPOSITORY                                   TAG         IMAGE ID       CREATED          SIZE
getting-started-v1_1                         latest      c3cf2766c545   4 seconds ago    1.12GB
```

## Building the Image with Multi-Stage Build with Slimmer Version

```
 docker build -t getting-started-v1_2 . -f Dockerfile2.multi
```

```
docker images
REPOSITORY
getting-started-v1_2                         latest      5ddbab822611   16 seconds ago   288MB
```

