CFLAGS=-Wall -O2
TARGET = ../bin/par

all : $(TARGET) ;

../bin :
	mkdir $@

$(TARGET) : par.c ../bin
	$(CC) $(CFLAGS) -o $@ $< -lm

clean:
	$(RM) $(TARGET)

