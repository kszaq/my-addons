OBJS = framebuffer.c newinput.c vncserver.c
CFLAGS += -Wall -std=c11 -mvectorize-with-neon-quad
LIBS := -static -lvncserver -lpng -ljpeg -lpthread -lz -lresolv

all: aml-vnc

aml-vnc: $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^ $(LIBS)

clean:
	$(RM) -rf
