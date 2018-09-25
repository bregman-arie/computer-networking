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
