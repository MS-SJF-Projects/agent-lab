FROM python:3.12-slim-bookworm AS base

RUN set -x

RUN apt-get update \
    && apt-get -y install curl \
    && apt-get -y install net-tools \
    && apt-get -y install procps \
    && apt-get -y install build-essential \
    && apt-get -y install docker.io \
    && apt-get -y install docker-compose \
    && apt-get -y install nodejs \
    && apt-get -y install npm


RUN pip install ipython ipykernel
RUN ipython kernel install --user --name promptflow

COPY requirements.txt .
RUN pip install -r requirements.txt

RUN set +x

CMD bash
