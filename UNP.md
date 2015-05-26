#Chapter 6
I/O multiplexing, why we need it?
When the process is blocked by an I/O event, for example, reading from standard input, it can not process other I/O event, which will cause processing failure. For example, a TCP client should both process standard input and socket descriptor which will cause process failure by either blocking.

#MSS and window size
How much data should we put into each segment? A primary determinant of how much data to send in a segment is the current status of the sliding window mechanism on the part of the receiver. However, a sgemetn size that will never be exceeded regardless of how large the current window is.

You can set the default value of window by changing SO_RCVBUF option in socket. However, the order should be followed. Listen and pre-connnect socket setting can be make sense.
