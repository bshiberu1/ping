This implementation of ping is reliant on the smoltcp rust crate and is meant for use in a ![no_std] environment

This application pings a specific IPv4 address and gets ping statistics.

Important: QEMU does not support the ICMP protocol by default so it's important to 
run this command: sudo sh -c "echo \"0 2147483647\" > /proc/sys/net/ipv4/ping_group_range"
in the environment prior to running this application

