# Seeed_reTerminal_Bridge_CAN_exmaple
### Example C code for using the CAN on the reTerminal Bridge.

To install VCAN0:

```sh
$ ip link add dev vcan0 type vcan
```

Use gcc to build examples:

One of the reTerminals compiles and runs the code that sends the data.
```sh
$ gcc cantransmit.c -o cantransmit
```

Another reTerminal compiles and runs the code that receives the data.
```sh
$ gcc canreceive.c -o canreceive
```

In addition to reading, you may want to filter out CAN frames that are not relevant. This happens at the driver level and this can be more efficient that reading each frame in a user mode application.

```sh
$ gcc canfilter.c -o canfilter
```