# docker-fail-images

## Crash Image

**Just exits with an error code**

Pull image:

```sh
docker pull ghcr.io/phartenfeller/crash-img:latest
```

Build youself from source:


```sh
cd ./crash-img
docker build . -t crash-img
docker run --rm  crash-img
```

## Stuck Image

**Never finishes**

Pull image:

```sh
docker pull ghcr.io/phartenfeller/stuck-img:latest
```

Build youself from source:


```sh
cd ./stuck-img
docker build . -t stuck-img
docker run -d --rm  stuck-img
```
