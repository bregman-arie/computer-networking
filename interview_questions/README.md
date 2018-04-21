# Interview Questions


## Network newbie

* What layers the OSI model has and what is the purpose of each one of them?

```
Application: user end (HTTP is here)
Presentation: establishes context between application-layer entities (Encryption is here)
Session: establishes, manages and terminates the connections
Transport: transfers variable-length data sequences from a source to a destination host (TCP & UDP are here)
Network: transfers datagrams from one network to another (IP is here)
Data link: provides a link between two directly connected nodes (MAC is here)
Physical: the electrical and physical spec the data connection (Bits are here)
```

* What delivery schemes are you familiar with?

```
Unitcast: One to one communication where there is one sender and one reciever.

Broadcast: Sending a message to everone in the network. The address ff:ff:ff:ff:ff:ff is used for broadcasting.
           Two common protocols which use broadcast are ARP and DHCP.

Multicast: Sending a message to a group of subscribers. It can be one-to-many or many-to-many.
```

* What is CSMA/CD? Is it used in modern ethernet networks?

```
CSMA/CD stands for Carrier Sense Multiple Access / Collision Detection.

Its primarly focus it to manage access to shared medium/bus where only one host can transmit
at a given point of time.

CSMA/CD algorithm:

    1. Before sending a frame, it checks whether another host already transmitting a frame.
    2. If no one transmitting, it starts transmitting the frame.
    3. If two hosts transmitted at the same time, we have a collision.
    4. Both hosts stop sending the frame and they send to everyone a 'jam signal' notifying everyone that a collision occured
    5. They are waiting for a random time before sending again
    6. Once each host waited for a raondom time, they try to send the frame again and so the process repeats.

Note: It is used in shared medium only so it is not very common to find it in used
in modern technology as today networks are using dedicated hardware and media.
```

* What is a switch?

```
A switch is a box of networking hardware with a large number of ports that forward Ethernet frames from one connected host to another.
When hosts first send frames over the switch, the switch doesn’t know which MAC address is associated with which port.
If an Ethernet frame is destined for an unknown MAC address, the switch broadcasts the frame to all ports.
The switch learns which MAC addresses are at which ports by observing the traffic.
Once it knows which MAC address is associated with a port, it can send Ethernet frames to the correct port instead of broadcasting.
The switch maintains the mappings of MAC addresses to switch ports in a table called a forwarding table or forwarding information base (FIB)
```

* What is a VLAN?

```
VLAN is a networking technology that enables a single switch to act as if it was multiple independent switches.
Specifically, two hosts that are connected to the same switch but on different VLANs do not see each other’s traffic.
```

* What is a trunk port?

```
A switchport that is configured to pass frames from all VLANs and tag them with the VLAN IDs is called a trunk port.
```

* What is ICMP? When is it used and how do you use it?

```
ICMP is a protocol used for sending control messages over an IP network.

For example: 
    * Router will send an ICMP packet to source when there is no route in routing table 
    * When IP packet is too large for the route to handle

CLI tools that make use of it: mtr and ping
```

* What is NAT?

```
NAT is a protocol used for modifying the destination or source addresses while the packet is in transit.
None of the involved hosts are aware of the process taking place.
```

## Linux Networking

* How do you initiate an ARP request manually?

```
arping -I eth0 192.40.2.52
```

* How to view the contents of the ARP cache?

```
arp -n
```


## OpenStack Neutron

* Name at least three network entities Neutron supports

```
Network
Port
Subnet
Router
Security Group
```

* What is the ML2 plugin?

```
ML2 plugin allow to simultaneously utilize several network technologies. For example, you can use both Openvswitch and Linux Bridge at the same time. Same applies for tunneling protocols like VXLAN and GRE. Before ML2 plugin was introduced you had to choose one mechanisem to work with.

ML2 allows doing that by using drivers. It distinguishes drives into two types: network type drivers and mechanism drivers.

Network type drives allow you to create a specific type of network. For example VXLAN, GRE, Geneve.

Mechanism drivers allow you to connect to or utilize existing systems, mechanisms like OpenvSwitch or Linux Bridge for example.
```

* What type of networks are you familiar with?

```
Provider networks which offer layer-2 connectivity to instances with optional support for DHCP and metadata services.
Project networks which allowprojects to manage networks without involving administrators. These networks are entirely virtual and
require virtual routers to interact with provider and external networks such as the Internet.
```
