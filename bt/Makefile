ifneq ($(KERNELRELEASE),)
	obj-m := rtk_btusb.o

else
	PWD := $(shell pwd)
	KVER := $(shell uname -r)
all:
	$(MAKE)  -C $(KDIR) M=$(PWD) modules

clean:
	rm -rf *.o *.mod.c *.mod.o *.ko *.symvers *.order *.a

endif
