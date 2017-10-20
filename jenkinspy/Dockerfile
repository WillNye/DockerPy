FROM jenkins/jenkins:lts
USER root
RUN apt-get -y update && apt-get install -y \
    git \
    python3 \
    python3-venv \
    python-pip \
    python3-dev \
    xvfb \
    build-essential \
    libssl-dev \
    libffi-dev \
    libpq-dev \
    libxml2-dev \
    libxslt1-dev \
    libldap2-dev \
    libsasl2-dev \
    sloccount

RUN pip install --upgrade pip

RUN wget https://github.com/mozilla/geckodriver/releases/download/v0.17.0/geckodriver-v0.17.0-linux64.tar.gz
RUN tar -xvzf geckodriver-v0.17.0-linux64.tar.gz
RUN mv geckodriver /usr/local/bin

ARG CACHEBREAK=1






