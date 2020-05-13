This application pings a specific IPv4 address and calculates ping statistics. This application is meant for use in a ![no_std] to diagnose network connectivity.

Similiarily to standard linux implemtations of ping, this implementation has builtin options such as:

"c", "count", "amount of echo request packets to send"

"i", "interval", "interval between packets being sent in miliseconds"

"t", "timeout", "maximum time between echo request and echo reply in milliseconds"

"s", "buffer size", "size of packet to send to target address"

