FROM nvidia/cuda:12.2.0-cudnn8-devel-ubuntu22.04

ENV PYTHON_VERSION=3.10.6
ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && apt install -y \
    python3.10 python3.10-venv python3.10-dev python3-pip \
    git wget curl libgl1 unzip nano ffmpeg libjpeg-dev \
    && ln -sf python3.10 /usr/bin/python3 \
    && python3 -m pip install --upgrade pip

RUN pip install torch==2.1.2 torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
RUN pip install xformers==0.0.23.post1

COPY docker/requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
