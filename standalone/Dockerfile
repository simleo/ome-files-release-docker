FROM ubuntu:14.04
MAINTAINER ome-devel@lists.openmicroscopy.org.uk

RUN apt-get update && apt-get -y install \
  curl \
  xz-utils \
  man \
  libjpeg-dev \
  libjbig-dev

COPY test_sample_data.sh /
