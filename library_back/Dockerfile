FROM python:3.9-alpine

ENV PYTHONUNBUFFERED 1

RUN apk --update add \
    build-base \
    postgresql \
    postgresql-dev \
    libpq

WORKDIR /back

COPY library_back/requirements.txt /back

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

COPY library_back/ /back