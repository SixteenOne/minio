# minio (containerized)

[![Build and Push Image to Dockerhub](https://github.com/SixteenOne/minio/blob/main/.github/workflows/docker.yml/badge.svg)](https://github.com/SixteenOne/minio/blob/main/.github/workflows/docker.yml)

This repository builds a Docker image from the official MinIO release and pushes the resulting image to Docker Hub.

## What this repo does
- Downloads or uses the official MinIO release (official upstream binary/release).
- Builds a container image that packages that MinIO release.
- Pushes the built image to a configured Docker Hub repository.

## Usage (quick)
Run a container for testing:
docker run -p 9000:9000 youruser/minio:latest server /data

Refer to MinIO docs for runtime flags and configuration.

## Note about MinIO docker releases
MinIO has stated that they are no longer providing further official Docker image releases. This repository packages the official MinIO release into a container image for users who require a Docker image, but it is not an official MinIO Docker distribution.