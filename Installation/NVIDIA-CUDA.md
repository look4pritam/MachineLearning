# NVIDIA CUDA

## Disable or Blacklist Nouveau

```sh
sudo bash -c "echo blacklist nouveau > /etc/modprobe.d/blacklist-nvidia-nouveau.conf"
sudo bash -c "echo options nouveau modeset=0 >> /etc/modprobe.d/blacklist-nvidia-nouveau.conf"

cat /etc/modprobe.d/blacklist-nvidia-nouveau.conf
```

```sh
sudo bash -c "echo blacklist nouveau > /etc/modprobe.d/blacklist.conf"
sudo bash -c "echo options nouveau modeset=0 >> /etc/modprobe.d/blacklist.conf"

cat /etc/modprobe.d/blacklist.conf
```

```sh
sudo update-initramfs -u
```

## NVIDIA CUDA

```sh
wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/cuda-ubuntu2004.pin
wget https://developer.download.nvidia.com/compute/cuda/11.6.2/local_installers/cuda-repo-ubuntu2004-11-6-local_11.6.2-510.47.03-1_amd64.deb

sudo cp cuda-ubuntu2004.pin /etc/apt/preferences.d/cuda-repository-pin-600

sudo dpkg -i cuda-repo-ubuntu2004-11-6-local_11.6.2-510.47.03-1_amd64.deb
sudo apt-key add /var/cuda-repo-ubuntu2004-11-6-local/7fa2af80.pub

sudo apt-get update
sudo apt-get -y install cuda
```
