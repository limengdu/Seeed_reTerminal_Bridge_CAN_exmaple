# Seeed_reTerminal_Bridge_CAN_exmaple
Example C code for SocketCAN on Linux

To install VCAN0:

$ ip link add dev vcan0 type vcan
Use gcc to build examples:

$ gcc cantransmit.c -o cantransmit

$ gcc canreceive.c -o canreceive

$ gcc canfilter.c -o canfilter
