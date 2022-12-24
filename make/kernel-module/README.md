# Cross-Compile Kernel Module

## Toolchain

```
# 32 bit
sudo apt-get install gcc-arm-linux-gnueabihf
# 64 bit
sudo apt-get install gcc-aarch64-linux-gnu
```

## Set Envs

```
export KDIR=~/path-to-kernel/linux
# 32 bit
export ARCH=arm
export CROSS_COMPILE=arm-linux-gnueabihf-

# 64 bit
export ARCH=arm64
export CROSS_COMPILE=aarch64-linux-gnu-
```

## Documentation
- https://embear.ch/blog/compiling-a-kernel-module