# define a imagem base
FROM python:3.9-alpine

# evita que a saída do python no terminal seja bufferizada
ENV PYTHONUNBUFFERED 1

# instala dependências do postgres
RUN apk --update add \
    build-base \
    postgresql \
    postgresql-dev \
    libpq \
    # dependências do pillow
    jpeg-dev \
    zlib-dev

# cria o diretório de trabalho
WORKDIR /code

# copia o restante do projeto para o diretório de trabalho
COPY . /code/