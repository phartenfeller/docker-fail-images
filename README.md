# docker-fail-images

## Crash Image

Just exits with an error code

```sh
cd ./crash-img
docker build . -t crash-img
docker run --rm  crash-img
```

## Stuck Image

Never finishes

```sh
cd ./stuck-img
docker build . -t stuck-img
docker run -d --rm  stuck-img
```
