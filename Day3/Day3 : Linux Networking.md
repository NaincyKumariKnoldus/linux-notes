###  How many tables are there in iptables? 
  IPTables has the following 5 tables: 
   1. `Filter Table` : Filter is default table for iptables. 
   2. `NAT table` : Iptable’s NAT table has the following built-in chains: 
       PREROUTING chain, POSTROUTING chain, OUTPUT chain 
   3. `Mangle table` : Iptables’s Mangle table is for specialized packet alteration. This alters QOS bits in the TCP header. 
   4. `Raw table` : Iptable’s Raw table is for configuration excemptions. 
   5. `Security table` : This table is used for Mandatory Access Control (MAC) networking rules, such as those enabled by the SECMARK and CONNSECMARK targets.


### What is prot, opt, in, out, source & destination?
  `prot`: Protocols. tcp, udp, icmp, etc., \
  `opt` : Special options for that specific rule. \
  `source`  : Source ip-address of the packet \
  `destination` : Destination ip-address for the packet 
  
### Why rules are added to the top?
Rules are added to top becuase whenever the packets are passed from the first rule it does not check the bottom rules.








### what type of rules we can add to the iptables?
 `Accept `- It lets the incoming packets from the source

`Reject `- It lets the other end know what port is unreachable.

`Drop ` It is used for connections to hosts we don’t want people to see.







### Can we block a website by its domain name only?
   Yes we can block a website by its domain name only by \
   `$ sudo iptables -A INPUT -s www.facebook.com -j DROP` 
   
   
### How can we save rules in iptables?
   The generic method of saving iptables rules is to use the command iptables-save, which writes to stdout. \
   ` $ iptables-save > /etc/network/iptables.rules`
   
### How can we persist rules in iptables?
1. Add rules to the iptables according to your requirment.

2. Verify that all the rules are present using the command “**iptables -L**“.

1. Add rules to the iptables according to your requirment.

2. Verify that all the rules are present using the command “**iptables -L**“.

3. Save the iptables.

   ```
   # service iptables save
   ```

   4-Restart the service.

   ```
   # service iptables restart
   ```

   5. Making service permanently **ON** using chkconfig.

   ```
   # chkconfig iptables on
   ```

   
   
   
   
### What are public & private keys?
   `Private key` : In Private key, the same key (secret key) is used for encryption and decryption. In this key is symmetric because the only key is copy or share by another party to decrypt the cipher text. It is faster than the public key cryptography.

   `Public Key`  : In Public key, two keys are used one key is used for encryption and another key is used for decryption. One key (public key) is used for encrypt the plain text to convert it into cipher text and another key (private key) is used by receiver to decrypt the cipher text to read the message.
   
### Difference between ufw & iptables?
   `iptables` : iptables provide a complete firewall solution that is both highly configurable and highly flexible.\
   `ufw` : The Uncomplicated Firewall (ufw) is a frontend for iptables.ufw aims to provide an easy to use interface for people unfamiliar with firewall concepts, while at the same time simplifies complicated iptables commands to help an administrator who knows what he or she is doing.






### How does ssh works?
  SSH is a client-server based protocol. This means the protocol allows a device requesting information or services (the client) to connect to another device (the server). 

When a client connects to a server over SSH, the machine can be controlled like a local computer. 

The server has a designated TCP port over which it monitors the network, waiting for clients to initialize the connection. Before a client connects and starts issuing SSH commands, it needs to pass the authentication process.\
Run the following command on a client machine to initiate an SSH connection: \
`$ ssh [username]@[server_ip_or_hostname]`

### Difference between HTTP & HTTPS?
| HTTP | HTTPS |
|----------------------------|-------------------------------------|
|HTTP stands for HyperText Transfer Protocol.| HTTPS for HyperText Transfer Protocol Secure.|
|In HTTP, URL begins with “http://”.|In HTTPs, URL starts with “https://”.|
|HTTP uses port number 80 for communication. | HTTPs uses 443 port number for communication.|
|HTTP is considered to be unsecure. | HTTPs is considered as secure.|
|HTTP works at Application Layer.| HTTPS works at Transport Layer.|
|In HTTP, Encryption is absent. | Encryption is present in HTTPS.|

### What is SSL?
 SSL stands for Secure Sockets Layer and, in short, it's the standard technology for keeping an internet connection secure and safeguarding any sensitive data that is being sent between two systems, preventing criminals from reading and modifying any information transferred, including potential personal details. The two systems can be a server and a client (for example, a shopping website and browser) or server to server (for example, an application with personal identifiable information or with payroll information).
 
### Difference between apt update & apt upgrade.
“apt-get update” updates the package sources list to get the latest list of available packages in the repositories and “apt-get upgrade” updates all the packages presently installed in our Linux system to their latest versions.

### Difference between apt & apt upgrade.
| apt update                                                   | apt upgrade                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| apt update is used to download package information from all configured sources. | apt upgrade is the command used to download and apply any available updates to your packages in a safe manner by not removing packages that are previously installed in a given Linux system |




### What do repositories contain in a Linux system?
 A Linux repository is a storage location from which your system retrieves and installs OS updates and applications. Each repository is a collection of software hosted on a remote server and intended to be used for installing and updating software packages on Linux systems. When you run commands such as “sudo apt update” or “sudo apt upgrade”, you may be pulling package information and package updates from a number of repositories.
 
 ### Difference between apt and apt-get?
 apt is a subset of apt-get and apt-cache commands providing necessary commands for package management.While apt does have some similar command options as apt-    get, it’s not backward compatible with apt-get.
 
 ### What does the number represent after the file permissions?
  The number represents the total number of files. \
  `-rwxrw-r-- 1` is a file with read, write and execute privileges for the owner. \
  `drwxr-xr-x 10` is a directory with 8 files. The extra 2 are . and ... Only the owner can create files in this directory, others can access which files are in the directory, and read the contents of those files if the privileges allow. \
  The number succeeding permission characters indicates the number of links if the node is a file, and number of "sub-nodes" if the node is a directory.


   
   
