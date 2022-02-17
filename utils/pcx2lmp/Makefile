TARGETS = ../bin/pcx2lmp ../bin/lmp2pcx

all: $(TARGETS)

../bin/%: %.c
ifeq "$(wildcard ../bin)" ""
	-mkdir $(dir $@)
endif
	$(CC) -o $@ -O2 -Wall $^ -lm

clean :
	$(RM) $(TARGETS)

