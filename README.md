# Readme

Oracle jdk 1.8

# Repository

- docker pull

```bash
docker pull primetoninc/jdk:1.8
docker pull primetoninc/jdk:latest
```

- dockerfile

```bash
FROM primetoninc/jdk:1.8

LABEL maintainer="lizw@primeton.com"

# TODO XXX
# build your application
# ...

ENTRYPOINT [ "/entrypoint.sh" ]
```
  
- docker build
  
```bash
git clone https://github.com/docker-repository/jdk.git
cd jdk
git checkout 1.8
git pull
docker build --rm -t your.registry.com/library/jdk:1.8 .
docker login your.registry.com
docker push your.registry.com/library/jdk:1.8
docker tag your.registry.com/library/jdk:1.8 your.registry.com/library/jdk:latest
docker push your.registry.com/library/jdk:1.8
```
