TARGET = mkupgimg.exe

CC = gcc
LD = $(CC)
CFLAGS=-c -std=gnu99

SOURCES=mkupgimg.c
OBJECTS=$(SOURCES:.c=.o)

all: $(TARGET)

$(TARGET): $(OBJECTS)
	$(LD) -o $@ $^ $(LDFLAGS)

%.o: %.c
	$(CC) $(CFLAGS) -o $@ $^

clean:
	rm -f $(OBJECTS) $(TARGET)
	
.PHONY: all clean	