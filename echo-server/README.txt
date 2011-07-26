Libevent based echo server example
-------------------------------------------------------------------------------

NOTE: These examples were built back in the libevent 1 days.  I
suggest new applications use libevent 2.  Excellent documentation for
the libevent 2 API can be found in the libevent book include an echo
server example.

    http://www.wangafu.net/~nickm/libevent-book/

First you must download and build libevent, you do not need to install
it.  
    libevent homepage: http://www.monkey.org/~provos/libevent/

To build libevent_echosrv:

    LIBEVENT=~/src/libevent-1.1a make

where LIBEVENT points to the location of your built libevent.

libevent_echosrv1

    This is the more basic of the 2 example apps.  It does not handle
    writing data the proper way for an event based non-blocking
    application.  For the sake of simplicity it echoes the data back
    to the socket as soon as it is received.

libevent_echosrv2

    This example puts read data onto a queue and schedules a write
    event.  It then waits for libevent to call the write callback
    before any data is written.  This demonstrates the proper way to
    handle writing in an event based non-blocking socket application.

USAGE

    Run the server:

        ./libevent_echosrc1

	OR

	./libevent_echosrv2

    Then telnet to localhost port 5555.  Anything you type will be
    echoed back to you.

--
Jason Ish <ish@unx.ca>
