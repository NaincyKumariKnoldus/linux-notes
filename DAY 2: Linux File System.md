### what are loop devices?
 A loop device, or it can be termed as vnode disk (vnd), and loopback file interface (lofi) is a device that helps the computer file to access block devices. Before using the dev loop, the existing file in the file system must be connected to it.
The “losetup” command-line tool is used to connect loop devices with the block devices. It helps to disconnect devices and check the query status of the dev loop. The syntax of the “losetup” command is: \
 `$ losetup {options}`
 
 ### Define squashfs file system.
 Squashfs is a compressed read-only file system for Linux. Squashfs compresses files, inodes and directories, and supports block sizes from 4 KiB up to 1 MiB for greater compression. A squashfs file system consists of a maximum of nine parts, packed together on a byte alignment. It uses zlib, lz4, lzo, or xz compression to compress files, inodes and directories. Inodes in the system are very small and all blocks are packed to minimise data overhead. Block sizes greater than 4K are supported up to a maximum of 1 Mbytes (default block size 128K).
 
 ### What are /dev/loop and /dev/tty?
`/dev` is the location of special or device files. It is a very interesting directory that highlights one important aspect of the Linux filesystem - everything is a file or a directory. 
`/dev/tty` stands for the controlling terminal (if any) for the current process (the process that uses "/dev/tty" in a command). To find out which tty's are attached to which processes use the "ps -a" command at the shell prompt (command line).

### What are Linux Signals?
In Linux, Signals are the interrupts that are sent to the program to specify that an important event has occurred. Events can vary from user requests to invalid memory access errors. Various signals, like the interrupt signal, means that the user has asked the program to perform something which is not present in the user flow of control.
There are two kinds of signals:
* `Maskable` : Maskable Signals are the signals that the user can change or ignore, for example, Ctrl +C.
* `Non-Maskable` : Non-Maskable Signals are the signals that the users cannot change or ignore. Non-Maskable signals mainly occur if a user is signaled for non-recoverable hardware errors.

### What are purpose of Hidden Files?
Files that exist on a computer, but don't appear when listing or exploring, are called hidden files. A hidden file is primarily used to help prevent important data from being accidentally deleted. \
On Linux, hidden files are files that are not directly displayed when performing a standard ls directory listing. Hidden files, also called dot files on Unix operating systems, are files used in order to execute some scripts or to store configuration about some services on your host. \
By default, all hidden files are not listed by the ls command. Any filename begins with a dot (.) becomes a hidden file. For example ~/.bashrc is a hidden file in Linux. Hidden files are often known as a dot file. And we can also delete that file. \
For listing dot file :     `ls -a | egrep '^\.'` \
For deleting dot file :         `rm -rfv /tmp/demo/.*`

### Why ext4 is faster than ext3?
Ext4 is functionally very similar to ext3, but brings large filesystem support, improved resistance to fragmentation, higher performance, and improved timestamps. Ext4 is also said to be slightly faster in sequential reads and writes.When it comes to file checking, EXT4 is quicker because unallocated blocks of data are marked as such and are simply skipped during disk check operations.

### What is swap and swap memory?
Swap space is a space on a hard disk that is a substitute for physical memory.It is also called a swap file. This interchange of data between virtual memory and real memory is called swapping and space on disk as “swap space”. \
swap memory is the dedicated amount of hard drive that is used whenever RAM runs out of memory. There is a memory management program in Linux that takes care of this process. Whenever RAM is short of memory, the memory management program looks for all those inactive blocks of data present in RAM that have not been used for a long time.

### Can 2 processes have the same process id?
Since PID is an unique identifier for a process, there's no way to have two distinct processes with the same PID.

###  Revisit Linux Directory Structure and each directory ?
`/` - Everything on your Linux system is located under the / directory, known as the root directory.
`/bin `: All the executable binary programs (file) required during booting, repairing, files required to run into single-user-mode, and other important, basic commands viz., cat, ls
`/boot `: Holds important files during the boot-up process , including Linux Kernel.
`/dev `: Contains device files for all the hardware devices on the machine.
`/etc ` : all the machine specific configuration files should be located in /etc.
`/home ` : Home directory of the users. Every time a new user is created, a directory in the name of the user is created within the home directory which contains other directories like Desktop, Downloads, etc.
`/lib `: Binaries found in /bin and /sbin often use shared libraries located in /lib.
`/media ` : Temporary mount directory is created for removable devices.
`/mnt `: Temporary mount directory for mounting file system.
`/opt ` : Optional is abbreviated as opt. Contains third party application software. Viz., Java, etc.
`/proc `: A virtual and pseudo file-system which contains information about a running process with a particular pid.
`/root `: This is the home directory of root user and should never be confused with /
`/sbin `: Contains binary executable programs to configure operating system , required by System Administrator , here s refers to sudo or super
`/srv `: Service is abbreviated as ‘srv‘. This directory contains server specific and service related files.
`/tmp ` :System’s Temporary Directory, Stores temporary files for user and system, till next boot.
`/usr `: stands for User System Resources. This directory contains most commands and executables files, libraries and documentation.
`/var `: Stands for variable. The contents of this file is expected to grow. This directory contains logs.







