CC = gcc
CFLAGS += -fPIC -std=c99
HEAP64_SIZE = 0
HEAP8_SIZE = 0

INSTALL_DIR = /home/bikram/.pyenv/versions/3.9.16/envs/trans/lib/python3.9/site-packages/prometeo/cmdline/..
SRCS += test.c
CFLAGS+=-I$(INSTALL_DIR)/include/blasfeo -I$(INSTALL_DIR)/include/prometeo
CFLAGS+=-DHEAP64_SIZE=$(HEAP64_SIZE)
CFLAGS+=-DHEAP8_SIZE=$(HEAP8_SIZE)
LIBPATH+=-L$(INSTALL_DIR)/lib/blasfeo -L$(INSTALL_DIR)/lib/prometeo


OBJS = 

casadi: 

sources: $(SRCS)
	$(CC) $(LIBPATH) -o test $(CFLAGS)  $(SRCS) $(OBJS) -lcpmt -lblasfeo -lm

all: casadi sources


clean:
	rm -f *.o test
