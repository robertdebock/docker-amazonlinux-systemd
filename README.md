Docker Amazon Linux Systemd
===========================

This Dockerfile can build containers capable to use systemd.

[![amazonlinux build status](https://img.shields.io/docker/cloud/build/robertdebock/amazonlinux.svg)](https://hub.docker.com/repository/docker/robertdebock/amazonlinux)

Branches
--------

This repository has multiple branches that relate to amazonlinux versions.

|Branch |amazonlinux Version|Docker image tag|
|-------|-------------------|----------------|
|master |2                  |latest          |
|1      |1                  |1               |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/amazonlinux
```
