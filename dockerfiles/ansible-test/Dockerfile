FROM alpine:latest
LABEL maintainer "Jack Hayhurst <jhayhurst@liquidweb.com>"

ARG CI_PROJECT_NAMESPACE
ARG CI_PROJECT_NAME

# update and install base packages
RUN apk --no-cache add \
	ca-certificates \
	python3 \
	py-paramiko \
	py-yaml \
	py-httplib2 \
	python3-dev \
	py3-pip \
	musl-dev \
	openssl-dev \
	libffi-dev \
	openssh-client \
	rsync \
	git \
	sshpass \
	gcc

COPY requirements.txt /
RUN pip install --upgrade pip && \
	pip install -r /requirements.txt

# COPY ansible.cfg /etc/ansible/ansible.cfg
