# Compile the STM32F10x Standard Peripheral Library
export

LIB_OUT = libleptonsdkoem.a

SRCS := $(shell find . -name *.[cs])

LIB_OBJS = $(sort $(patsubst %.c,%.o,$(SRCS))) 

.PHONY: all
.PHONY: clean

all: $(LIB_OUT)

$(LIB_OUT): $(LIB_OBJS)
	$(AR) $(ARFLAGS) $@ $(LIB_OBJS)

clean:
