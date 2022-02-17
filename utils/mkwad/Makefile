TARGET = ../bin/mkwad

$(TARGET) : mkwad.c
ifeq "$(wildcard ../bin)" ""
	mkdir $(dir $@)
endif
	$(CC) -o $@ -O2 -Wall $^ -lm

clean :
	$(RM) $(TARGET)
