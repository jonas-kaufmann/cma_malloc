PWD   := $(shell pwd)
obj-m := cma_malloc.o 
# KDIR  := /home/jonask/Repos/simbricks/images/kernel/linux-5.15.93
KDIR  := /home/jonask/Repos/simbricks/images_arm64/kernel/linux-5.15.93
kernel_options := ARCH=arm64 CROSS_COMPILE=aarch64-linux-gnu-
# kernel_options :=


default:
	$(MAKE) $(kernel_options) -C $(KDIR) M=$(PWD) modules

clean: 
	$(MAKE) $(kernel_options) -C $(KDIR) M=$(PWD) clean
