modified so command:

tcpser -v 25232 -s 9600 -p 6400 -l 7

will now work for use with socat + retro hardware emulator

after running above command do

socat -v -d -d pty,rawer,link=/tmp/com1 tcp4:localhost:25232
