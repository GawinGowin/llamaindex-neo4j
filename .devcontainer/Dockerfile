FROM mcr.microsoft.com/devcontainers/python:3.10-bullseye

ENV PYTHONUNBUFFERED 1
ENV DEBIAN_FRONTEND=noninteractive

# [Optional] If your requirements rarely change, uncomment this section to add them to the image.
COPY requirements.txt /
RUN pip3 --disable-pip-version-check --no-cache-dir install -r /requirements.txt \
   && rm -rf /requirements.txt

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update \
#     && apt-get -y install --no-install-recommends <your-package-list-here>
