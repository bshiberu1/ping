This implementation of ping is reliant on the smoltcp rust crate and is meant for use in a ![no_std] environment

This application pings a specific IPv4 address and gets ping statistics. This can be used to diagnose network
connectivity and similiarily to standard linux implemtations has certain builtin options:

"c", "count", "amount of echo request packets to send"
"i", "interval", "interval between packets being sent in miliseconds"
"t", "timeout", "maximum time between echo request and echo reply in milliseconds"
"s", "buffer size", "size of packet to send to target address"

Important: QEMU does not support the ICMP protocol used by echo requests("pings") by default so it's important to 
run this command: sudo sh -c "echo \"0 2147483647\" > /proc/sys/net/ipv4/ping_group_range" in the environment 
prior to running this application

