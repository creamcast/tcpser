modified to fix error when using tcp port for VICE RS232

tcpser -v 25232 -s 9600 -p 6400 -l 7

*use socat to connect a virtual serial port

socat -v -d -d pty,rawer,link=/tmp/com1 tcp4:localhost:25232
