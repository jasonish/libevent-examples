CFLAGS =	-I$(LIBEVENT) -Wall
LIBS =		$(LIBEVENT)/.libs/libevent.a -lrt

all: libevent_echosrv1 libevent_echosrv2


libevent_echosrv1: libevent_echosrv1.c
	$(CC) $(CFLAGS) -g -O2 -o $@ libevent_echosrv1.c $(LIBS)

libevent_echosrv2: libevent_echosrv2.c
	$(CC) $(CFLAGS) -g -O2 -o $@ libevent_echosrv2.c $(LIBS)

clean:
	rm -f libevent_echosrv1 libevent_echosrv2 *~

