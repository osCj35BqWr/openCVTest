FROM python:3.7-slim

# opencv-devのインストール
RUN apt-get update -y && apt-get install -y libopencv-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
    
WORKDIR /tmp/work
COPY requirements.txt ${PWD}
RUN pip install -r requirements.txt
