FROM registry
RUN apk add apache2-utils
#RUN echo "proxy:" >> /etc/docker/registry/config.yml
#RUN echo "  remoteurl: https://registry-1.docker.io" >> /etc/docker/registry/config.yml
RUN mkdir /docker-registry
WORKDIR /docker-registry
RUN mkdir data
RUN mkdir auth
WORKDIR auth