### What are Daemon Applications?
A daemon (also known as background processes) is a [Linux] program that runs in the background. Almost all daemons have names that end with the letter "d". For example, [httpd] the daemon that handles the Apache server, or, [sshd] which handles [SSH] remote access connections. Linux often start daemons at boot time. Shell scripts stored in [/etc/init.d] directory are used to start and stop daemons.

### What .d represent after a file?
"d" stands for directory and such a directory is a collection of configuration files which are often fragments that are included in the main configuration file. The point is to compartmentalize configuration concerns to increase maintainability.

### What is in the host file?
The host file stores the hostname and ip address.This file is an ASCII text file. It contains IP addresses separated by a space and then a domain name. Each address gets its own line.

### How port forwarding works?
Port forwarding is a technique that is used to allow external devices access to computers services on private networks.SSH Port forwarding is used to forward ports between a local and a remote Linux machine using SSH protocol.Local port forwarding is the most common type of port forwarding. It is used to let a user connect from the local computer to another server, i.e. forward data securely from another client application running on the same computer as a Secure Shell (SSH) client.

### How can we connect without IP to AWS instance?
Go into the EC2 dashboard, then in the NETWORK & SECURITY menu go to Elastic IPs. Click on Allocate a new address. Right click on the new IP and select Associate address. Associate it with your EC2 instance that doesn't have an elastic IP.

### What is SCP & what does this command do?
The SCP is a network protocol, based on the BSD RCP protocol, which supports file transfers between hosts on a network. SCP uses Secure Shell (SSH) for data transfer and uses the same mechanisms for authentication, thereby ensuring the authenticity and confidentiality of the data in transit.
The scp command copies files or directories between a local and a remote system or between two remote systems. You can use this command from a remote system (after logging in with the ssh command) or from the local system. The scp command uses ssh for data transfer.
