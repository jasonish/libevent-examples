Libevent buffered event echo server example
-------------------------------------------------------------------------------

First you must download and build libevent, you do not need to install
it.  
    libevent homepage: http://www.monkey.org/~provos/libevent/

To build libevent_echosrv:

    LIBEVENT=~/src/libevent-1.1a make

where LIBEVENT points to the location of your built libevent.

USAGE

    Run the server:

        ./libevent_echosrv_buffered

    Then telnet to localhost port 5555.  Anything you type will be
    echoed back to you.

--
Jason Ish <ish@unx.ca>
