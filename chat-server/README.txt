A simple chat server using libevent.
-------------------------------------------------------------------------------

Requires libevent 2.0+.

First you must download and build libevent, you do not need to install
it.  

    libevent homepage: http://www.monkey.org/~provos/libevent/

To build libevent_echosrv:

    LIBEVENT=~/src/libevent-2.0.12-stable make

where LIBEVENT points to the location of your built libevent.

USAGE

    Run the server:

        ./chat-server

    Then telnet to localhost port 5555 from multiple terminals.
    Anything you type in one terminal will be sent to the other
    connected terminals.

--
Jason Ish <ish@unx.ca>
