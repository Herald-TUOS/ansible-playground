FROM python:3.11-bullseye

RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir ansible

RUN apt update && apt install -y openssh-server openssh-client