```powershell
# for gcc
gcc -v    # check the version of gcc
sudo apt-get install gcc-8
sudo rm -rf /usr/bin/gcc
sudo ln -s /usr/bin/gcc-8 /usr/bin/gcc

# for cmake
cmake --version

## 添加签名密钥
wget -O - https://apt.kitware.com/keys/kitware-archive-latest.asc 2>/dev/null | sudo apt-key add -
## 将存储库添加到您的源列表并进行更新
sudo apt-add-repository 'deb https://apt.kitware.com/ubuntu/ bionic main'
sudo apt-get update
## 然后再使用apt安装就是最新版本的cmake啦
sudo apt install cmake

# for python environment
conda create -n ngp python=3.7 -y
conda activate ngp

# for optix
# following the guidance on NVIDIA website
```