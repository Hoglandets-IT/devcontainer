ARG PYTHON_VERSION=3.12
ARG OS_VERSION=bookworm
FROM mcr.microsoft.com/devcontainers/python:${PYTHON_VERSION}-${OS_VERSION}

COPY install.sh /tmp/install.sh

ARG ACCEPT_EULA=Y
RUN bash /tmp/install.sh && rm /tmp/install.sh && apt-get clean && rm -rf /var/lib/apt/lists/*