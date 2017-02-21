FROM ubuntu:14.04
MAINTAINER ome-devel@lists.openmicroscopy.org.uk

RUN apt-get update && apt-get -y install \
  curl \
  xz-utils \
  man \
  libjpeg-dev \
  libjbig-dev \
  libboost1.55-all-dev \
  libxerces-c-dev \
  libtiff5-dev \
  libxalan-c-dev

COPY test_sample_data.sh /
