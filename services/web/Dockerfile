FROM python:3.10.5-slim-buster

# set user dir
WORKDIR /tmp/data/work/


# set environment variables
# Prevents Python from writing pyc files to disc
ENV PYTHONDONTWRITEBYTECODE 1

# Prevents Python from buffering stdout and stderr
ENV PYTHONUNBUFFERED 1

# install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /tmp/data/work/requirements.txt
RUN pip install -r requirements.txt

COPY . /tmp/data/work