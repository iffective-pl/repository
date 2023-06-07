FROM registry
ENV DOCKER_PASSWORD $password
RUN apt install apache2-utils -y
RUN mkdir /docker-registry
WORKDIR /docker-registry
RUN mkdir data
RUN mkdir auth
WORKDIR auth
RUN htpasswd -Bc registry.password docker $password