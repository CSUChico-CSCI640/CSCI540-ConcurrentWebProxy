CC = gcc
CFLAGS = -Wall -g 
LDFLAGS = -lpthread

OBJS = proxy.o csapp.o echo.o echoclient.o echoserveri.o

all: proxy echoclient echoserver 

proxy: $(OBJS)
	gcc $(CFLAGS) proxy.o csapp.o -o proxy $(LDFLAGS)

echoserver: $(OBJS)
	gcc $(CFLAGS) echoserveri.o echo.o csapp.o -o echoserver $(LDFLAGS)

echoclient: $(OBJS)
	gcc $(CFLAGS) echoclient.o csapp.o -o echoclient $(LDFLAGS)
	
clean:
	rm -f proxy echoclient echoserver proxy.log *.o *~


