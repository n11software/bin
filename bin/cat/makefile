PROG=cat

CC=x86_64-hydra-gcc
CFLAGS=-O2 -pedantic --std=c89 -g

$(PROG): cat.o
	$(CC) -o $@ cat.o $(CFLAGS)

clean:
	rm -rf *.o $(PROG)

.c.o:
	$(CC) $(CFLAGS) -c $*.c

cat.o: cat.c
