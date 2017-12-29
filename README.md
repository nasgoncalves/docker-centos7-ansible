# Docker Centos 7 Ansible

Latest Centos 7 (+ systemd) & Ansible releases.

[Docker Hub](https://hub.docker.com/r/nasg/centos7-ansible/)

```
docker pull nasg/centos7-ansible
```

## Build
```
docker build --rm -t nasg/centos7-ansible:latest .
```

## Run
```
docker run --cap-add SYS_ADMIN --privileged -v /sys/fs/cgroup:/sys/fs/cgroup:ro -d --name ansible nasg/centos7-ansible
docker exec -it ansible bash
```
