FROM python:3.9-bullseye

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONBURRERED=1

WORKDIR /backend

COPY requirements.txt requirements.txt

RUN pip install --upgrade pip \
    &&pip install -r requirements.txt

COPY . /backend