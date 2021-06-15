# docker-fail-images

I use these images to test some docker container orchestration logic.

## Crash Image

**Just exits with an error code**

Use image:

```sh
docker pull ghcr.io/phartenfeller/crash-img:latest
docker run --rm ghcr.io/phartenfeller/crash-img:latest
```

Build youself from source:


```sh
cd ./crash-img
docker build . -t crash-img
docker run --rm  crash-img
```

## Stuck Image

**Never finishes**

Use image:

```sh
docker pull ghcr.io/phartenfeller/stuck-img:latest
docker run --rm -d ghcr.io/phartenfeller/stuck-img:latest
```

Build youself from source:


```sh
cd ./stuck-img
docker build . -t stuck-img
docker run -d --rm  stuck-img
```
