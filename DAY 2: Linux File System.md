### what are loop devices?
 A loop device, or it can be termed as vnode disk (vnd), and loopback file interface (lofi) is a device that helps the computer file to access block devices. Before using the dev loop, the existing file in the file system must be connected to it.
The “losetup” command-line tool is used to connect loop devices with the block devices. It helps to disconnect devices and check the query status of the dev loop. The syntax of the “losetup” command is: \
 `$ losetup {options}`
 
 ### Define squashfs file system.
 Squashfs is a compressed read-only file system for Linux. Squashfs compresses files, inodes and directories, and supports block sizes from 4 KiB up to 1 MiB for greater compression. A squashfs file system consists of a maximum of nine parts, packed together on a byte alignment. It uses zlib, lz4, lzo, or xz compression to compress files, inodes and directories. Inodes in the system are very small and all blocks are packed to minimise data overhead. Block sizes greater than 4K are supported up to a maximum of 1 Mbytes (default block size 128K).
 
 ### What are /dev/loop and /dev/tty?
`/dev` is the location of special or device files. It is a very interesting directory that highlights one important aspect of the Linux filesystem - everything is a file or a directory. 
`/dev/tty` stands for the controlling terminal (if any) for the current process (the process that uses "/dev/tty" in a command). To find out which tty's are attached to which processes use the "ps -a" command at the shell prompt (command line).



