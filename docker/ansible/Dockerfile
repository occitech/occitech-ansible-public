FROM python:3.6-alpine3.7

RUN apk add --update gcc musl-dev libffi-dev openssl-dev ca-certificates git rsync openssh-client docker
RUN pip install --upgrade pip
RUN pip install ansible
RUN pip install pyyaml
RUN pip install docker-compose
