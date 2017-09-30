light-python
==========

Debian 9 based, production-ready and lightweight Python3 container.

Docker Hub: https://hub.docker.com/r/camilo0365r/light-python/

----------

## Features
- Based on the `stretch-slim` tag from the official [Debian Docker registry](https://hub.docker.com/_/debian/).
- Python 3.6 with `glibc` instead of `musl`. This solves compatibility when compiling certain libraries from source.
- Just the necessary system dependencies to deploy production-ready containers.
- Downloaded Image size approx. 130MB (Official images can be as big as 600MB+).

## Why another Python image?
At the time of writing (October 2017) the official Python [Docker registry](https://hub.docker.com/_/python/) does not include a barebones and lightweight Python image based on **glibc** (not musl as in Alpine-based images) and Debian 9 (Stretch).

## Image size comparison vs official Python registry

| Image                   | Size in Docker Hub | Downloaded Size |
|-------------------------|--------------------|-----------------|
| **light-python:3.6.1**  | 50MB               | 140MB           |
| python:slim             | 80MB               | 206MB           |
| python:jessie           | 274MB              | 690MB           |
| python:stretch          | 350MB              | 909MB           |


## Usage

```bash
$ docker pull camilo0365r/light-python:latest
```
