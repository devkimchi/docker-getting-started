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
 docker build -t getting-started-v2 . -f Dockerfile.multi
```

## Result:

```
 docker images
REPOSITORY                                   TAG         IMAGE ID       CREATED          SIZE
getting-started-v2                           latest      7b3d14a1ad95   7 seconds ago    201MB
```

## Building the Image with Multi-Stage Build with Slimmer Version

