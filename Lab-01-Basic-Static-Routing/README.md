# Lab 01 – Basic Static Routing

-----

##  Overview

This lab demonstrates the implementation of a basic static routing topology using GNS3. The network consists of two Cisco routers and two virtual PCs connected across two separate LANs.
The routers were configured with IP addresses, and static routes were added to enable communication between the two networks. Connectivity was verified using the `ping` command between routers and end devices.

-----

##  Objectives

The objectives of this lab are to:

- Build a basic network topology using GNS3.
- Configure IP addresses on routers and PCs.
- Establish communication between two different LANs.
- Configure static routes on both routers.
- Verify network connectivity using the `ping` command.
- Verify interface status using the `show ip interface brief` command.

-----
  
##  Network Topology

The following topology was created in GNS3 for this lab.

![Network Topology](topology.png)

-----

##  IP Addressing


| Device | Interface | IP Address | Subnet Mask |
|---------|-----------|------------|-------------|
| R1 | Fa0/0 | 192.168.10.1 | 255.255.255.0 |
| R1 | Fa0/1 | 192.168.20.3 | 255.255.255.0 |
| R2 | Fa0/0 | 192.168.10.2 | 255.255.255.0 |
| R2 | Fa2/0 | 192.168.30.4 | 255.255.255.0 |
| PC1 | NIC | 192.168.20.5 | 255.255.255.0 |
| PC2 | NIC | 192.168.30.6 | 255.255.255.0 |

-----

##  Configuration Steps


1. Created the network topology in GNS3.
2. Connected two Cisco routers and two VPCS hosts.
3. Configured IP addresses on all router interfaces.
4. Assigned IP addresses and default gateways to both PCs.
5. Configured static routes on both routers.
6. Saved the running configuration.
7. Verified connectivity using ping.

-----

##  Verification

The following verification tests were successfully completed.

- Router R1 successfully pinged Router R2.
- Router R2 successfully pinged Router R1.
- PC1 successfully communicated with PC2.
- PC2 successfully communicated with PC1.
- Static routes were verified using `show ip route`.
- Interface status was verified using `show ip interface brief`.

  -----

##  Lessons Learned

After completing this lab, I learned how to:

- Build a basic network topology using GNS3.
- Configure router interfaces.
- Assign IP addresses to routers and PCs.
- Configure static routes.
- Verify interface status using `show ip interface brief`.
- Verify routing tables using `show ip route`.
- Test connectivity using the `ping` command.
- Save router configurations.

  -----

##  Conclusion

This lab successfully demonstrated the implementation of static routing between two separate LANs using Cisco routers in GNS3. After configuring IP addressing and static routes, end-to-end connectivity was successfully verified between both networks.
