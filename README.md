# Ubuntu-18.04-docker-images-systemd

Ubuntu 18.04 docker images systemd systemctl enable

RUN :

download all files and then :

docker build -t ubuntu:18.04 .

docker run -itd --name systemd --security-opt seccomp=unconfined --tmpfs /run --tmpfs /run/lock -v /sys/fs/cgroup:/sys/fs/cgroup:ro ubuntu:18.04
