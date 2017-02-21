# ome-files-release-docker

Docker images for reviewing ome-files releases.

```
docker run --rm -it -v /ome:/ome:ro simleo/ome-files-release-standalone
docker run --rm -it -v /ome:/ome:ro simleo/ome-files-release-platform
```

**NOTE:** on macOS you might need to add `/ome` to the list of sharable directory trees, see https://docs.docker.com/docker-for-mac/osxfs.

From the Docker container (example for release 0.3.1, standalone):

```
curl -O http://downloads.openmicroscopy.org/ome-files-cpp/0.3.1/21/binaries/ome-files-standalone-bundle-0.3.1-Release-Ubuntu14.04-x86_64-b21.tar.xz
tar xf ome-files-standalone-bundle-0.3.1-Release-Ubuntu14.04-x86_64-b21.tar.xz
export PATH="/ome-files-standalone-bundle-0.3.1-Release-Ubuntu14.04-x86_64-b21/bin:${PATH}"
export MANPATH="/ome-files-standalone-bundle-0.3.1-Release-Ubuntu14.04-x86_64-b21/share/man:${MANPATH}"
```
