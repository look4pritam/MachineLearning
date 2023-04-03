# Docker-CE

- Install curl.

```sh
sudo apt install curl

curl https://get.docker.com | sh \
  && sudo systemctl --now enable docker
```

- Add user to 'docker' group.

```sh
sudo groupadd docker

sudo usermod -aG docker $USER
```

- Reboot the machine.
