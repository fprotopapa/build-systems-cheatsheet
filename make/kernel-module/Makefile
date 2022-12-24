obj-m := myfoomodule.o

# Export or specify in Makefile
# export ARCH=arm
# export CROSS_COMPILE=arm-linux-gnueabihf-

# Export kernel path before running make when cross-compiling
KERNELDIR ?= /lib/modules/$(shell uname -r)/build

all default: modules
install: modules_install

modules modules_install help clean:
$(MAKE) -C $(KERNELDIR) M=$(shell pwd) $@