###  How many tables are there in iptables? 
  IPTables has the following 4 built-in tables: 
   1. `Filter Table` : Filter is default table for iptables. 
   2. `NAT table` : Iptable’s NAT table has the following built-in chains: 
       PREROUTING chain, POSTROUTING chain, OUTPUT chain 
   3. `Mangle table` : Iptables’s Mangle table is for specialized packet alteration. This alters QOS bits in the TCP header. 
   4. `Raw table` : Iptable’s Raw table is for configuration excemptions. 
### What is prot, opt, in, out, source & destination?
  `prot`: Protocols. tcp, udp, icmp, etc., \
  `opt` : Special options for that specific rule. \
  `source`  : Source ip-address of the packet \
  `destination` : Destination ip-address for the packet \
  `in` : 
### Why rules are added to the top?
