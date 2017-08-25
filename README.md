# Readme

    Oracle jdk 1.8

# Repository

- docker pull

    docker pull primetoninc/jdk:1.8
    docker pull primetoninc/jdk:latest

- dockerfile

    FROM primetoninc/jdk:1.8

    LABEL maintainer="lizw@primeton.com"

    # build your application
    # ...


- docker build
  
    git clone https://github.com/orgs/docker-repository/jdk.git
    cd jdk
    docker build --rm -t your.registry.com/library/jdk:1.8 .
    docker login your.registry.com
    docker push your.registry.com/library/jdk:1.8
    docker tag your.registry.com/library/jdk:1.8 your.registry.com/library/jdk:latest
    docker push your.registry.com/library/jdk:1.8
