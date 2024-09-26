# Campus Network Topology
### In this project, I created a simple campus network topology. The configuration in this topology was done as described below. Through this project, protocols such as Dynamic Trunking Protocol (DTP) and Spanning Tree Protocol (STP) became more understandable for me. I gained experience with VLANs. I verified the structure of the topology I built by using protocols like CDP and LLDP. I configured the ports between switches as trunks. I assigned VLANs to the ports between PCs and switches and set them as access ports. I assigned IP addresses to each VLAN. I used PortChannel to combine the ports between two switches named core1 and core2 into a single logical port. I configured the core1 and core2 switches as roots according to the VLANs. For access security, I set passwords on both the switch and router so that users who don’t know the password cannot configure them. The many other tasks I performed are as follows:

### Configured the network as follows:
1) Configured Host Names
2) Shutdown unused interfaces
3) Configured enable password and vty passwords of cisco
(in this order conf t-enable password cisco- line vty 0 4-password cisco)
4) Using VTP mode transparent and domain ccna
5) Add VLANS 10,20,30,100 to the VLAN database
6) Configured ports between switches as trunks
7) Configured access ports on links to PCs
8) Using CDP and LLDP to verify links
9) Verified which ports are forwarding and blocking (spanning tree)
10) Optimized spanning tree with Core1 being root for odd VLANs (vlan1 vlan10 vlan30)
and Core2 the root for even VLANS(vlan20 vlan100).
Before the configuration, there could be a
 heavy load on the g1/0/23 port between core1 and core2, 
as communication was only established through this port while the others were blocked.

11) Configured Etherchannel on the core switches
12) Core switches  supported layer 3 interVLAN routing:
VLAN 1 = Core 1 = 10.1.1.251/24, Core 2 = 10.1.1.252/24
VLAN 10 = Core 1 = 10.1.10.251/24, Core 2 = 10.1.10.252/24
VLAN 20 = Core 1 = 10.1.20.251/24, Core 2 = 10.1.20.252/24
VLAN 30 = Core 1 = 10.1.30.251/24, Core 2 = 10.1.30.252/24
VLAN 100 = Core 1 = 10.1.100.251/24, Core 2 = 10.1.100.252/24
13) Access layer switches will  have management IP addresses in VLAN 1:
Switch 1 = 10.1.1.1/24
Switch 2 = 10.1.1.2/24
Switch 3 = 10.1.1.3/24


 
 
