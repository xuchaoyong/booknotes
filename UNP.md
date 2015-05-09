#Chapter 6
I/O multiplexing, why we need it?
When the process is blocked by an I/O event, for example, reading from standard input, it can not process other I/O event, which will cause processing failure. For example, a TCP client should both process standard input and socket descriptor which will cause process failure by either blocking.
