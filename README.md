# Dockerfile Best Practices Bug

This repository demonstrates a common bug in Dockerfiles: using an unspecified base image (`ubuntu:latest`). This can lead to inconsistencies and security vulnerabilities across builds.

## Bug
The `Dockerfile` uses `ubuntu:latest`, leading to unpredictable behavior.  Updates to the `ubuntu:latest` image could break builds and introduce unexpected security risks.

## Solution
The `Dockerfile.fixed` file provides a corrected version, specifying a specific version of Ubuntu instead.