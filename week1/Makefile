CC = gcc
CFLAGS =
LDFLAGS = 

.SUFFIXES : .c .o
.c.o :
	$(CC) -c $(CFLAGS) $<

ALL = helloworld_server helloworld_client low_open low_read

all: $(ALL)

helloworld_server: helloworld_server.o
	$(CC) -o $@ $< $(LDFLAGS)

helloworld_client: helloworld_client.o
	$(CC) -o $@ $< $(LDFLAGS)

low_open: low_open.o
	$(CC) -o $@ $< $(LDFLAGS)

low_read: low_read.o
	$(CC) -o $@ $< $(LDFLAGS)


clean:
	rm -rf *.o $(ALL)
