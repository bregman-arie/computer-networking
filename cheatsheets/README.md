# Cheat Sheets

## Linux

* Retrieve the MAC address and IP of a specific NIC

```
ip link show <interface_name>

Example:

$ ip link show enp0s23

enp0s23: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP mode DEFAULT group default qlen 1000
 link/ether 08:00:29:c4:62:56 brd ff:ff:ff:ff:ff:ff
```

* Show all interfaces and their addresses (IP and MAC)

```
ip addr

# Shortcut: ip a
```
