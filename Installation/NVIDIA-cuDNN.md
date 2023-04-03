# [NVIDIA cuDNN](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html)

- Download 'cudnn-local-repo-ubuntu2004-8.4.0.27_1.0-1_amd64.deb' from NVIDIA website.

```sh
sudo dpkg -i cudnn-local-repo-ubuntu2004-8.4.0.27_1.0-1_amd64.deb 
sudo apt-key add /var/cudnn-local-repo-ubuntu2004-8.4.0.27/7fa2af80.pub

sudo apt-get update
sudo apt-get install libcudnn8=8.4.0.27-1+cuda11.6
sudo apt-get install libcudnn8-dev=8.4.0.27-1+cuda11.6
sudo apt-get install libcudnn8-samples=8.4.0.27-1+cuda11.6
```
