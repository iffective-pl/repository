FROM registry
ENV DOCKER_PASSWORD $password
RUN apk add apache2-utils
RUN mkdir /docker-registry
WORKDIR /docker-registry
RUN mkdir data
RUN mkdir auth
WORKDIR auth
RUN htpasswd -Bc registry.password docker $password