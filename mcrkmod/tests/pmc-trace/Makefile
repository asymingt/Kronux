APP1=rk_trace_pmc_set
APP2=rk_trace_pmc_get

KERNEL_DIR = ../../../

CC = $(CROSS_COMPILE)gcc
CCFLAGS := -I$(KERNEL_DIR) -I$(KERNEL_DIR)/include/rk -DCONFIG_RK -lrt -DARCH_$(ARCH) -D_GNU_SOURCE
CCFLAGS += -O3

all: 
	$(CC) -o $(APP1)  $(APP1).c $(CCFLAGS) 
	$(CC) -o $(APP2)  $(APP2).c $(CCFLAGS) 

clean:
	rm -f $(APP1)
	rm -f $(APP2)

