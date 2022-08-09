# NVIDIA Jarvis

## [VirtualBox](VirtualBox.md)

## [Ubuntu 20.04](Ubuntu-20.04.md)

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

