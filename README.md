# SymPy Dockerfile

[![Build Status](https://travis-ci.org/aktech/sympy-docker.svg?branch=master)](https://travis-ci.org/aktech/sympy-docker)

This repository contains Dockerfile of Sympy for Docker's automated build
published to the public Docker Hub Registry.

## Usage

* Pull image from dockerhub

```bash
$ docker pull aktech/sympy
Using default tag: latest
latest: Pulling from aktech/sympy
f49cf87b52c1: Already exists
7b491c575b06: Already exists
b313b08bab3b: Already exists
51d6678c3f0e: Already exists
09f35bd58db2: Already exists
0f9de702e222: Already exists
73911d37fcde: Already exists
99a87e214c92: Already exists
6ba03e115097: Pull complete
Digest: sha256:82728d3a4b648817d436a60416a39e01f45d1136e5cdd651dccd83ee8236947a
Status: Downloaded newer image for aktech/sympy:latest
```

* Check Image

```bash
$ docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
aktech/sympy        latest              d5db373de6b2        3 minutes ago       741MB
```

* Play

```bash
docker run -it d5db373de6b2
Type "help", "copyright", "credits" or "license" for more information.
Python 3.6.4 (default, Dec 21 2017, 01:35:12)
[GCC 4.9.2] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import sympy
>>> sympy.__version__
'1.1.1'
>>>
```
