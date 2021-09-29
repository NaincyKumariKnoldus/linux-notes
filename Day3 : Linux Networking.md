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
  `in` :                                           \
### Why rules are added to the top?








### what type of rules we can add to the iptables?








### Can we block a website by its domain name only?
   Yes we can block a website by its domain name only by \
   `$ sudo iptables -A INPUT -i facebook.com -j DROP` 
   
   
### How can we save rules in iptables?
   The generic method of saving iptables rules is to use the command iptables-save, which writes to stdout. \
   ` $ iptables-save > /etc/network/iptables.rules`
   
### How can we persist rules in iptables?
   
   
   
   
   
### What are public & private keys?
   `Private key` : In Private key, the same key (secret key) is used for encryption and decryption. In this key is symmetric because the only key is copy or share by another party to decrypt the cipher text. It is faster than the public key cryptography.

   `Public Key`  : In Public key, two keys are used one key is used for encryption and another key is used for decryption. One key (public key) is used for encrypt the plain text to convert it into cipher text and another key (private key) is used by receiver to decrypt the cipher text to read the message.
   
### Difference between ufw & iptables?

   
   
