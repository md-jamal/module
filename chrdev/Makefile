PWD := $(shell pwd)
obj-m := test.o
test-objs := char.o

default:
	$(MAKE) -C $(KER_SRC) M=$(PWD) modules

clean:
	$(MAKE) -C $(KER_SRC) M=$(PWD) clean

install:test.ko
	-cp test.ko $(INSTALL_DIR)
