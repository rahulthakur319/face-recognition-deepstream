# Starting the Project

This document describes how to launch the development container for working on the face recognition DeepStream application.

## Prerequisites

Ensure Docker is installed with NVIDIA Container Toolkit and your GPU drivers are correctly configured.

## Starting the Container

Run the following command from the root of the repository:

```bash
docker run -it --gpus all \
  -v $(pwd):/workspace/face-recognition-deepstream \
  rahulthakur-deepstream-7.1-py:latest
```

This command pulls the pre-configured DeepStream 7.1 Python image and mounts the current repository into `/workspace/face-recognition-deepstream` inside the container. You can then run `python3 main.py` or other tools from within the container.

