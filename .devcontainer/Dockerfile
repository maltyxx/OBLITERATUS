FROM nvidia/cuda:12.6.3-cudnn-devel-ubuntu24.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y --no-install-recommends \
    python3 \
    python3-pip \
    python3-venv \
    python3-dev \
    git \
    && rm -rf /var/lib/apt/lists/*

# Make python3 the default python
RUN ln -sf /usr/bin/python3 /usr/bin/python

WORKDIR /workspaces/oblteratus
