# targets
obj-m := xt_layer7.o

PWD := $(shell pwd)

default:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) modules

clean:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) clean

install:
	mkdir -p ${ROOT}/lib/custom_modules/
	cp xt_layer7.ko ${ROOT}/lib/custom_modules/
