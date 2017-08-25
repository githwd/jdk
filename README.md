# Readme

Oracle jdk 1.7

# Repository

- docker pull

```bash
docker pull primetoninc/jdk:1.7
```
  
- dockerfile

```bash
FROM primetoninc/jdk:1.7

LABEL maintainer="lizw@primeton.com"

# TODO XXX
# build your application
# ...

ENTRYPOINT [ "/entrypoint.sh" ]
```
  
- docker build

```bash
git clone https://github.com/orgs/docker-repository/jdk.git
cd jdk
git checkout 1.7
git pull
docker build --rm -t your.registry.com/library/jdk:1.7 .
docker login your.registry.com
docker push your.registry.com/library/jdk:1.7
docker push your.registry.com/library/jdk:1.7
```