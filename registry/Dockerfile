FROM registry
RUN --mount=type=secret,id=DOCKER_PASSWORD
RUN apk add apache2-utils
RUN mkdir /docker-registry
WORKDIR /docker-registry
RUN mkdir data
RUN mkdir auth
WORKDIR auth
RUN htpasswd -Bc registry.password docker | cat /run/secrets/DOCKER_PASSWORD