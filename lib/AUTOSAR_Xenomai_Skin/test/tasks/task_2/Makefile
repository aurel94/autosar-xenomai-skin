XENO_CONFIG := /home/matthieuk/Documents/Embedded/Xenomai/Buildroot/buildroot-2016.05/output/host/usr/arm-buildroot-linux-gnueabihf/sysroot/usr/bin/xeno-config
CFLAGS := $(shell $(XENO_CONFIG) --autosar --cflags)
LDFLAGS := $(shell $(XENO_CONFIG) --autosar --ldflags)
CC := $(shell $(XENO_CONFIG) --cc)

EXECUTABLE := task_2

all: $(EXECUTABLE)

%: %.c
	 $(CC) -o $@ $< $(CFLAGS) $(LDFLAGS)
