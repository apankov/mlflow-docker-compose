FROM python:3.14-slim

RUN apt update && apt install -y --no-install-recommends \
    sqlite3 libsqlite3-dev && \
    rm -rf /var/lib/apt/lists/*

# Install python packages
COPY requirements.txt /tmp
RUN pip install -r /tmp/requirements.txt
