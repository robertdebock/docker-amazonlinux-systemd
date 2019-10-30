Docker Amazon Linux Systemd
===========================

This Dockerfile can build containers capable to use systemd.

Branches
--------

This repository has multiple branches that relate to amazonlinux versions.

|Branch |amazonlinux Version|Docker image tag|
|-------|-------------------|----------------|
|master |2                  |latest          |

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
  robertdebock/docker-amazonlinux-systemd
```
