# wbroker
The message distribution system is similar to the pub / sub function of the zmq library, but the function is simpler than that of zmq, and it is purely an asynchronous message broker.


1. Currently only supports tcp protocol.

2. The bottom copy of the message uses a zero copy strategy.

3. Only responsible for the delivery of the message flow, not the integrity of the package.

# Test Data:

The average packet is 20 bytes: proxy speed is 12,700,000 / s, cpu: 9%, memory: 113m.

The average packet is 50 bytes: proxy speed 7,300,000 / s, cpu: 11%, memory: 132m.
