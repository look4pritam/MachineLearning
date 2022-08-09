# [NVIDIA TensorRT](https://docs.nvidia.com/deeplearning/tensorrt/install-guide/index.html)

- Download 'nv-tensorrt-repo-ubuntu2004-cuda11.6-trt8.4.0.6-ea-20220212_1-1_amd64.deb' from NVIDIA website.

```sh
sudo dpkg -i nv-tensorrt-repo-ubuntu2004-cuda11.6-trt8.4.0.6-ea-20220212_1-1_amd64.deb
sudo apt-key add /var/nv-tensorrt-repo-cuda11.6-trt8.4.0.6-ea-20220212/7fa2af80.pub

sudo apt-get update
sudo apt-get install tensorrt 
```

```sh
python3 -m pip install numpy
sudo apt-get install python3-libnvinfer-dev

sudo mv /usr/lib/python3.8/dist-packages/* /opt/tis/lib/python3.8/site-packages/.
```

```sh
sudo apt-get install uff-converter-tf
```
