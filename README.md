Dockerfile for ubuntu 18.04 with systemd


## Usage

You can run container with:
```bash
docker run -dt -v /sys/fs/cgroup:/sys/fs/cgroup:ro --tmpfs /run --tmpfs /run/lock --security-opt seccomp=unconfined  ultransible/ubuntu_18_04_systemd name_container 
```
## Build the container

If you want to re-build the container, you have to clone the repo and trigger the building:
```bash
git clone https://github.com/ultransible/ubuntu_18_04_systemd.git
cd ubuntu_18_04_systemd
docker build .
```
