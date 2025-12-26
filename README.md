# AMD ISP4 Camera Module Installation

Enables the AMD ISP4 camera on systems with AMD Ryzen AI processors.

## Prerequisites

Install kernel headers, build tools, and b4:

```bash
# Arch
sudo pacman -S base-devel linux-headers b4

# Ubuntu/Debian
sudo apt install build-essential linux-headers-$(uname -r) b4

# Fedora
sudo dnf install kernel-devel kernel-headers gcc make b4
```

## Install

```bash
make
sudo make install
```

## Rebuild after kernel update

```bash
make clean
make
sudo make install
```
