FROM ubuntu:20.04

USER root

RUN apt -y update && \
    apt -y install python3-pip openssh-client openssl

RUN pip install --upgrade pip && \
    pip install ansible && \
    ansible-galaxy collection install azure.azcollection && \
    pip install -r ~/.ansible/collections/ansible_collections/azure/azcollection/requirements-azure.txt
