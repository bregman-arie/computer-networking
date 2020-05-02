Checklists
==========

Check your educational progress with the following checklists

Note: similar questions can be found in [interview questions](https://github.com/bregman-arie/computer-networking/tree/master/interview_questions/README.md) page with answers

## Network Newbie

- [ ] **OSI model**
  - [ ] What layers the OSI model has and what is the purpose of each one of them?

- [ ] **Ethernet**
  - [ ] What is CSMA/CD and how it works?

- [ ] **MAC address**
  - [ ] What is it used for? Is it unique?
  - [ ] How many bits are in a MAC address?

- [ ] **IP address**
  - [ ] What is it used for? Is it unique worldwide?
  - [ ] What are the two parts of an IP address?
  - [ ] How many bits are in an IP address?

- [ ] **Subnets**
  - [ ] Two hosts are on the same subnet if they have the same '_____'
  - [ ] What is a netmask?
  - [ ] What two syntaxes exist for expressing a netmask?

- [ ] **ARP**
  - [ ] Which layer of the OSI model do ARP belong to?
  - [ ] What ARP table includes?
  - [ ] Give an example of how ARP protocol works

- [ ] **IP**
  - [ ] What it defines?
  - [ ] What is a routing table? When is it being used?

- [ ] **TCP**
  - [ ] What are the differences between TCP and UDP? When would you prefer to use TCP over UDP?
  - [ ] What is a "three-way handshake"?

- [ ] **UDP** 
  - [ ] Why UDP considered to be unreliable when compared to TCP?
  - [ ] Which layer of the OSI model do UDP belong to?

- [ ] **DHCP**
  - [ ] How DHCP client locates the DHCP server?
  - [ ] Does the client has to be on the same local network as the server?
  - [ ] How the exchange between client and the server looks like? what steps are included?
  - [ ] Is it using TCP or UDP?
  - [ ] What ports is it using?

- [ ] **Network Devices**
  - [ ] What is a HUB?
  - [ ] What is a Switch?
    - [ ] Forwarding table or (aka forwarding information base)
  - [ ] What is a Router?
  - [ ] What are differences between the three devices above?

- [ ] **Delivery schemes**
  - [ ] What is unicast?
  - [ ] What is multicast?
  - [ ] What is broadcast?
    - [ ] What is the broadcast address?
    - [ ] What protocols use broadcast?
    - [ ] What is a broadcast domain?

- [ ] **VLAN**
  - [ ] What are the advantages of using VLAN?
  - [ ] What is the range for VLAN IDs?
  - [ ] What is a trunk port?

- [ ] **Topologies**
  - [ ] Bus topology
  - [ ] Ring topology
  - [ ] Star topology
  - [ ] Tree topology

- [ ] **IP**
  - [ ] What layer of OSP model it belongs to?
  - [ ] IPv4
  - [ ] IPv6
    - [ ] Why IPv6 is needed if IPv4 exists?

- [ ] **ICMP**
  - [ ] What is it used for?
  - [ ] How do you use it?

- [ ] **NAT**
  - [ ] What is it and why it's needed?
  - [ ] What is SNAT? how it is different from NAT?
  - [ ] What is DNAT? how it is different from SNAT?

## Intermediate

- [ ] **Routing**
  - [ ] Distance Vector Routing
    - [ ] "Count-to-infinity" problem
  - [ ] Dijkstra's algorithm

- [ ] **TCP**
  - [ ] Silly window syndrome
    - [ ] Nagle's algorithm
    - [ ] Clark's solution

## Linux Networking

- [ ] **Commands**
  - [ ] ping
  - [ ] ip addr
  - [ ] ip neigh
  - [ ] ip link
  - [ ] ip route
  - [ ] ip netns
  - [ ] ethtool
  - [ ] netstat
  - [ ] traceroute
  - [ ] tcpdump
  - [ ] mtr

- [ ] **ARP**
  - [ ] How to view the contents of the ARP cache?
  - [ ] How to initiate an ARP request manually?

- [ ] **MTU**
  - [ ] How to see what is the MTU of a given interface?
  - [ ] How do you set MTU?

- [ ] **Namespaces**
  - [ ] How to create & delete namespaces?
  - [ ] How to enter a specific namespace?

- [ ] **Routing*
  - [ ] How to display the routing table?
  - [ ] How to print the IP address of each router that an IP packet traverses along its path to its destination?

- [ ] **ICMP**
  - [ ] How do you use it?

## Academic Level

- [ ] **Digital Modulation**
  - [ ] What is Amplitude Shift keying?
  - [ ] What is Frequency Shift Keying?
  - [ ] What is Phase Shift keying?

- [ ] **Multiplexing**
  - [ ] What is it used for and how it works?

- [ ] **Wireless networks**
  - [ ] The hidden terminal problem
  - [ ] The exposed terminal problem
  - [ ] **MACA**
    - [ ] What is RTS?
    - [ ] What is CTS?

- [ ] **ALOHA**
  - [ ] Pure
  - [ ] Slotted

- [ ] **Noisy-channel coding theorem**
  - [ ] Shannon capacity/limit

- [ ] **CSMA**
  - [ ] The Binary Exponential Backoff Algorithm

- [ ] **Stop and Wait**

- [ ] **The adaptive tree walk**

- [ ] **Cryptography**
  - [ ] Symmetric
  - [ ] Asymmetric
  - [ ] Digital Signature

- [ ] **Error Detection**
  - [ ] Parity Bit
  - [ ] Checksum
  - [ ] CRC code

- [ ] Data transmission
  - [ ] Piggybacking

- [ ] **Error Correction**
    - [ ] Hamming Code
    - [ ] Reed Solomon code
    - [ ] The NASA binary convolutional code
    - [ ] Low-Density Parity Check code

## Cloud Networking (OpenStack Neutron)

- [ ] **Components**
  - [ ] API Server
  - [ ] Plugins
  - [ ] Agents
  - [ ] Messaging Queue

- [ ] **Entities**
  - [ ] Network
  - [ ] Router
  - [ ] Port
  - [ ] Subnet
  - [ ] Security Group

- [ ] **ML2 Plugin**
  - [ ] What is it used for?
  - [ ] Explain type drivers
  - [ ] Explain mechanism drivers

- [ ] **dnsmasq***

- [ ] **Floating IP**

- [ ] **Provider Network**
