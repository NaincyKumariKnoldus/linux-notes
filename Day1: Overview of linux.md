### What is the GNU project?
   GNU stands for GNU's not Unix. The GNU project is a mass collaborative initiative for the development of free software. The original purpose of the GNU project was the creation of a free operating system. Free, in a software context, does not necessarily mean free of cost. The freedom referred to is the ability of anyone who wishes to run, copy, distribute, study, change and improve the software. According to the GNU Linux project, the Linux operating system's kernel is Linux but all other elements of the system are GNU.  According to the project,  neither OS exists independently and, as such Linux would more appropriately be called GNU Linux.
### Difference between Unix and Linux?
 * Linux is an open-source operating system which is freely available to everyone. Whereas Unix is an operating system which can be only used by its copywriters.
 * Linux is just the kernel, whereas Unix is a complete package of Operating systems.
 * BASH is the Linux default shell. It offers support for multiple command interpreters. Unix Originally made it work in Bourne Shell. However, it is now compatible with many other software.
 * Linux source is available to the general public whereas unix source code is not available to anyone.
 
 ### What is UEFI? Difference between UEFI and BIOS?
 The BIOS (basic input/output system) is a firmware component stored in nonvolatile memory, usually a flash chip.The BIOS loads the boot loader, which is the first software component loaded during the boot process. \
 The boot loader is stored in the hard drive, together with the operating system and applications. \
 UEFI stands for Unified Extensible Firmware Interface. It does the same job as a BIOS, but with one basic difference: it stores all data about initialization and startup in an .efi file, instead of storing it on the firmware.
 UEFI was designed to overcome many limitations of the old BIOS, including: \
 * UEFI supports drive sizes upto 9 zettabytes, whereas BIOS only supports 2.2 terabytes.
 * UEFI has discrete driver support, while BIOS has drive support stored in its ROM, so updating BIOS firmware is a bit difficult.
 * UEFI offers security like "Secure Boot", which prevents the computer from booting from unauthorized/unsigned applications. This helps in preventing rootkits, but also hampers dual-booting, as it treats other OS as unsigned applications.
 * UEFI runs in 32bit or 64bit mode, whereas BIOS runs in 16bit mode. So UEFI  is able to provide a GUI (navigation with mouse) as opposed to BIOS which allows navigation only using the keyboard.
 
 ### When should I go for Ubuntu & when for other systems?
1. Free of Cost \
Downloading and installing Ubuntu is free, and costs only time to install it. One can just download from the internet or can create an ISO bootable disk, and after it, the environment is ready to launch.
2. Privacy \
In comparison to Windows, Ubuntu provides a better option for privacy and security. The best advantage of having Ubuntu is that we can acquire the required privacy and additional security without having any third party solution. Risk of hacking and various other attacks can be minimized by using this distribution.
3. Working with Partitions of hard drives \
Linux live CD and Gparted enable to divide the hard disk into partitions. This feature is also applicable when your system is a dual or triple boot. Otherwise, the partition is helpful in migration to solid state drive or more spacious drive. Apart from this, wiping of data can be easily done in Ubuntu.
4. Free Apps \
Ubuntu provides a lot of free apps to explore the world of opportunities, refreshments, and enjoyment. 
5. User-Friendly \
Ubuntu is as easy as the Windows operating system. There is a well-known myth about Ubuntu is that Ubuntu is developed for developers and coders only. But the actual fact is, Ubuntu is a beautiful desktop operating system and can be used by any common computer user.
6. Say Bye to Antivirus \
Risk of having a virus or malware is minimal, that reduces the cost of anti-virus software. Antivirus is also a reason for the slowness of the computer system and affects performance badly

### What are the various operating systems & their uses?
`MS-DOS`:which is short for Microsoft Disk Operating System is a non-graphical command line operating system developed for IBM compatible computers with x86 microprocessor. The operating system used a command line interface for the user to input commands to navigate, open and manipulate files on their computer. \
`Windows Operating System` : Windows is an operating system designed by Microsoft to be used on standard x86 Intel and AMD processors. It provides an interface, known as a graphical user interface(GUI) which eliminates the need to memorize commands for the command line by using a mouse to navigate through menus, dialog boxes, buttons, tabs, and icons. The operating system was named windows since the programs are displayed in the shape of a square. \
`LINUX Operating System` : The Linux OS is an open source operating system project that is a freely distributed, cross-platform operating system developed based on UNIX. This operating system is developed by Linus Torvalds. The name Linux comes from the Linux kernel. It is basically the system software on a computer that allows apps and users to perform some specific task on the computer. 

### What are getty commands?
`getty [ [ -r | -u | -U ] [ -d ] [ -H HeraldString ] [ -M motdFile ] [ -N ] ] PortName`

The getty command sets and manages terminal lines and ports. The getty command is run by the init command. The getty command is linked to the Terminal State Manager program. The Terminal State Manager program provides combined terminal control and login functions. \
You can configure the getty command to create your home directory at your login if you do not have a home directory already. The getty command calls the mkuser.sys command to create the home directory and customize the account. To enable this capability, set the mkhomeatlogin attribute of the usw stanza in the /etc/security/login.cfg file to true. The getty command is not entered on the command line. \
The file /usr/sbin/getty contains the getty command.

### What are Uname commands?
The command ‘uname‘ displays the information about the system.
Syntax: `uname [OPTION]`
1. `-a option`: It prints all the system information in the following order: Kernel name, network node hostname, kernel release date, kernel version, machine hardware name, hardware platform, operating system.
2. `-s option`: It prints the kernel name.
3. `-n option`: It prints the hostname of the network node(current computer).
4. `-r option`: It prints the kernel release date.
5. `-v option`: It prints the version of the current kernel.
6. `-m option`: It prints the machine hardware name.
7. `-p option`: It prints the type of the processor.
8. `-i option`: It prints the platform of the hardware.
9. `-o option`: It prints the name of the operating system.














