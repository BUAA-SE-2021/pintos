# Pintos 环境搭建

> Author: Muyung, YinghaoZhu

## 依赖安装

我所使用的实验环境为 VMware Workstation 16 Player (免费) 上运行的 Ubuntu 16.04

- [Download VMware Workstation 16 Player](https://www.vmware.com/cn/products/workstation-player/workstation-player-evaluation.html)
- [Download Ubuntu 16.04](http://releases.ubuntu.com/xenial/)
  - 选择 ubuntu-16.04.7-desktop-amd64.iso

### 安装 GNU binutils

安装成功后，终端运行 `i386-elf-objdump -i`，应输出：

```sh
BFD header file version (GNU Binutils) 2.21.1
elf32-i386
    (header little endian, data little endian)
    i386...
```

如果未出现这一信息，则需要安装 `binutils` ：

首先下载该依赖包：终端执行 `wget http://ftpmirror.gnu.org/binutils/binutils-2.21.1.tar.bz2`

解压并安装：

```sh
tar xjf binutils-2.21.1.tar.bz2
cd binutils-2.21.1
./configure --prefix=/usr/local --target=i386-elf --disable-werror
make
sudo make install # 这一步权限必不可少
cd ..
```

### 安装 Bochs

这里采用的 Bochs 版本是 2.6.7，而非 Pintos 推荐的 2.2.6，因为过旧版本的 bochs 已经无法通过新版本 gcc 的编译。

这里先将可能用到的依赖都安装验证一遍：

```sh
sudo apt-get update # 更新 apt 库
sudo apt-get -y install build-essential # -y 参数自动确认 (Y/n)
sudo apt-get -y install xorg-dev
sudo apt-get -y install bison
sudo apt-get -y install libgtk2.0-dev
sudo apt-get -y install libc6:i386 libgcc1:i386 libstdc++5:i386 libstdc++6:i386
sudo apt-get -y install libncurses5:i386
sudo apt-get -y install g++-multilib
```

[下载 bochs02.6.7 链接](https://sourceforge.net/projects/bochs/files/bochs/2.6.7/)

点击"bochs-2.6.7.tar.gz"下载，解压并安装：

```sh
tar xzf bochs-2.6.7.tar.gz
cd bochs-2.6.7
./configure --enable-gdb-stub
make
sudo make install # 这一步权限必不可少
```