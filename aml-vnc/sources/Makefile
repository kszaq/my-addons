OBJS = framebuffer.c newinput.c vncserver.c
LIBS := -lvncserver -lpng -ljpeg -lpthread -lssl -lcrypto -lz -lresolv -lsystemd

all: aml-vnc

aml-vnc: $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^ $(LIBS)

clean:
	$(RM) -rf
