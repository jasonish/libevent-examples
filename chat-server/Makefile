CFLAGS =	-I$(LIBEVENT) -Wall

LIBS =		$(LIBEVENT)/.libs/libevent.a -lrt

chat-server: chat-server.c
	$(CC) $(CFLAGS) -o $@ $^ $(LIBS)

clean:
	rm -f chat-server *~
