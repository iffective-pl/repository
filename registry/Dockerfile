FROM registry
RUN apk add apache2-utils
RUN mkdir /docker-registry
WORKDIR /docker-registry
RUN mkdir data
RUN mkdir auth
WORKDIR auth
RUN htpasswd -b -cB registry.password docker 7DqdgwYb8M