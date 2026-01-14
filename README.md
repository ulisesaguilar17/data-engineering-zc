# data-engineering-zc

## Docker comands

Check Docker is configure correctly

```bash
docker run -it ubuntu
```

Docker download image ubuntu:

```bash
docker run ubuntu
```

Update python

```bash
apt update
```

Check python Version:

```bash
python3 -V
```

## Different Base Images

There are other base images besides `hello-world` and `ubuntu`. For example, Python:

```bash
docker run -it --rm python:3.9.16
```


```bash
docker run -it --rm --entrypoint=bash python:3.9.16-slim
# Dame un Ubuntu/Debian chiquito con Python 3.9.16 y ábreme una consola bash, y cuando termine destrúyelo
```

