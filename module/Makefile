ifndef KERNEL_DIR
$(error KERNEL_DIR is not set)
endif

KERNEL_OPTIONS ?=
CCFLAGS_Y ?=

PWD := $(shell pwd)
obj-m := cma_malloc.o  
ccflags-y := $(CCFLAGS_Y)

default:
	$(MAKE) $(KERNEL_OPTIONS) -C $(KERNEL_DIR) M=$(PWD) modules

clean: 
	$(MAKE) $(KERNEL_OPTIONS) -C $(KERNEL_DIR) M=$(PWD) clean
