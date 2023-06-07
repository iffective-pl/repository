FROM registry
ENV DOCKER_PASSWORD $password
RUN apt install apache2-utils -y
MKDIR /docker-registry
WORKDIR /docker-registry
MKDIR data
MKDIR auth
WORKDIR auth
RUN htpasswd -Bc registry.password docker $password