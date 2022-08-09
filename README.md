# NVIDIA Jarvis

## [VirtualBox](VirtualBox.md)

## Ubuntu 20.04
- Download an iso image from [link](https://releases.ubuntu.com/20.04/ubuntu-20.04.4-desktop-amd64.iso).
- /boot - 1024 MB
- swap  - 8192 MB
- /     - remaining

## Docker-CE

```sh
sudo apt  install curl

curl https://get.docker.com | sh \
  && sudo systemctl --now enable docker
```

```sh
sudo groupadd docker

sudo usermod -aG docker $USER
```

