CFLAGS =	-I$(LIBEVENT) -Wall
LIBS =		$(LIBEVENT)/.libs/libevent.a -lrt

libevent_echosrv_buffered: libevent_echosrv_buffered.c
	$(CC) $(CFLAGS) -o $@ libevent_echosrv_buffered.c $(LIBS)
clean:
	rm -f libevent_echosrv_buffered *~
