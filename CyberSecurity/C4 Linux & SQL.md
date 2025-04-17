# Module 1 **Introduction To Operating Systems**

> ## Operating System
> Interface between computer hardware and the user

> ## Hardware
> Physical components of a computer

> ## Legacy Operating Systems
> A legacy operating system is an operating system that is outdated but still being used.

> ## Booting the computer
> When you boot, or turn on, your computer, either a BIOS or UEFI microchip is activated. The Basic Input/Output System (BIOS) is a microchip that contains loading instructions for the computer and is prevalent in older systems. The Unified Extensible Firmware Interface (UEFI) is a microchip that contains loading instructions for the computer and replaces BIOS on more modern systems.


![Completing a task](image-6.png)

> ### Application
> A program that performs a specific task

> ## What is a virtual machine?
> A virtual machine (VM) is a virtual version of a physical computer.  <br>
> The term “virtual” refers to machines that don’t exist physically, but operate like they do because their software simulates physical hardware. Virtual systems don’t use dedicated physical hardware. Instead, they use software-defined versions of the physical hardware. This means that a single virtual machine has a virtual CPU, virtual storage, and other virtual hardware. Virtual systems are just code.

> ### Virtualization
> Virtualization is the process of using software to create virtual representations of various physical machines.

> ## Benefits of Virtual Machines
> - Security
> - Efiiciency

> ### Hypvervisor
>  Virtual machines can be managed with a software called a hypervisor. Hypervisors help users manage multiple virtual machines and connect the virtual and physical hardware. Hypervisors also help with allocating the shared resources of the physical host machine to one or more virtual machines. Ex: Kernel-based Virtual Machine (KVM)

> ### User Interface
> A program that allows the user to control the functions of the operating system

> ## Graphical User Interface (GUI)
> A user interface that uses icons on the screen to manage different tasks on the computer
>> **Basic GUI components**
>> - Start Menu
>> - Task bar
>> - Desktop with icons and shortcuts

> ## Command-line Interface (CLI)
> A text-based user interface that uses commands to interact with the computer 


# Moduel 2 **The Linux Operating System**

> ## Linux
> An open-source operating system

> ## Components of Linux | Linux Architecture
> - **User** <br>
> The person interacting with the computer 
> - **Applications**<br>
> A program that performs a specific task
> - **Shell**<br>
> The command-line interpreter 
> - **Filesystem Hierarchy Standard (FHS)**<br>
> The component of the Linux OS that organizes data
> - **Kernel**<br>
> The component of the Linux OS that manages proccesses and memory
> - **Hardware**<br>
> The physical components of a computer


> ## Distributions
>> Different versions of Linux
>
> ## Parent Distributions
> - Red Hat Enterprise Linux (CentOS)
> - Slackware (SUSE)
> - Debian (Ubuntu and KALI LINUX)
>
> #### Penetration Test
> A simulated attack that helps identify vulnerabilities in systems, networks, websites, applications and processes
>
> ### KALI LINUX
> KALI LINUX ™ is an open-source distribution of Linux that is widely used in the security industry. This is because KALI LINUX ™, which is Debian-based, is pre-installed with many useful tools for penetration testing and digital forensics.
> #### Few Penetration testing tools in Kali Linux
>> - Metasploit
>> - Burp Suite
>> - John the Ripper
>
> #### Digital Forensics
> The practice of collecting and analyzing data to determine what has happened after an attack
>
> #### Digital forensic tools in Kali Linux
>> - tcpdump
>> - Wireshark
>> - Autopsy
>
> ### Ubuntu 
> Ubuntu is an open-source, user-friendly distribution that is widely used in security and other industries. It has both a command-line interface (CLI) and a graphical user interface (GUI). Ubuntu is also Debian-derived and includes common applications by default. 
>
> ### Parrot
> Parrot is an open-source distribution that is commonly used for security. Similar to KALI LINUX ™, Parrot comes with pre-installed tools related to penetration testing and digital forensics.It is based on Debian.
>
> ### Red Hat® Enterprise Linux®
> Red Hat Enterprise Linux is a subscription-based distribution of Linux built for enterprise use. Red Hat is not free, which is a major difference from the previously mentioned distributions. Because it’s built and supported for enterprise use, Red Hat also offers a dedicated support team for customers to call about issues.
>
> ### AlmaLinux
> AlmaLinux is a community-driven Linux distribution that was created as a stable replacement for CentOS. CentOS was an open-source distribution that is closely related to Red Hat, and its final stable release, CentOS 8, was in December 2021. CentOS used source code published by Red Hat to provide a similar platform. AlmaLinux is designed to be a drop-in replacement for CentOS 8. This ensures that applications and configurations that worked on CentOS will continue to function on AlmaLinux. 

> ## Package Manager
> A package is a piece of software that can be combined with other packages to form an application. <br>
>  A **package manager** is a tool that helps users install, manage, and remove packages or applications. Linux uses multiple package managers. 
>
> Different package managers typically use different file extensions. <br>For example, *Red Hat Package Manager (RPM)* has files which use the *.rpm* file extension, such as *Package-Version-Release_Architecture.rpm.* Package managers for *Debian-derived Linux distributions*, such as *dpkg*, have files which use the *.deb* file extension, such as *Package_Version-Release_Architecture.deb.*
>
> In addition to package managers like RPM and dpkg, there are also package management tools that allow you to easily work with packages through the shell. Two notable tools are the Advanced Package Tool (APT) and Yellowdog Updater Modified (YUM).
> - **Advanced Package Tool (APT)** <br>
> APT is a tool used with Debian-derived distributions. It is run from the command-line interface to manage, search, and install packages.
> - **Yellowdog Updater Modified (YUM)** <br>
> YUM is a tool used with Red Hat-derived distributions. It is run from the command-line interface to manage, search, and install packages. YUM works with .rpm files.

> ## Shell
> The command-line interpreter
>
> #### Command
> An instruction telling the computer to do something
>
> ### Different types of shells
> - Bourne-Again Shell (bash)
> - C Shell (csh)
> - Korn Shell (ksh)
> - Enhanced C shell (tcsh)
> - Z Shell (zsh)
> 
> ### Input and Output in the shell
>
> **- echo** <br>
> A Linux command that outputs a specified string of text <br><br>
> ***String data**: Data Consisting of an ordered sequence of characters* <br>
>
>> **Standard output:** the respons given by OS throught the shell <br>
>> **Standard error:** error messages returned by the OS through the shell <br>


# Module 3 Linux Commands in the Bash Shell

> #### Types of things seccurity analyysts require to do
> - work with server logs
> - Navigate, manage, and analyze files remotely
> - Verify and configure users and group access
> - Give authorization and set file permissions 

**Bash:** Default cell in most linux distributions

## Commands in Linux
> #### Directory navigation commands
> - **pwd** <br>
> Prints the working directory onto the screen
>
> - **ls**
> Displays the names of files and directories in the current working directory
> 
> - **cd**
> Navigates between directories <br>
> TIP:  You can use the relative file path and enter `cd ..` to go up one level in the file structure.
>
> #### File-related commands
> - **cat**
> Displays conent of a file
>
> - **head**
> Displays just the beginning of a file, by default 10 lines <br>
> TIP: If you want to change the number of lines returned by head, you can specify the number of lines by including `-n`. For example, if you only want to display the first five lines of the updates.txt file, enter `head -n 5 updates.txt`.
> 
> - **tail**
> This commmand is the opposite of *`head`*. i.e. it is used to display the ennd of a file, by default 10 lines. <br>
> Note: `tail` is commonly used to read the most recent information in log file
>
> - **less**
> *less* returns the content of a file one page at a time. It changes the terminal window to display the contents of the file, one page at a time. This  allows the user to easily move forward and backward through the content. <br>
> Once the content is accessed using *`less`*, you can use keyboard to control your movement through the file: <br>
> *`space bar`*: Moves forward one page <br>
> *`b`*: Moves back one page <br>
> *`down arrow`*: moves forward one line <br>
> *`up arrow`*: moves back one line <br>
> *`q`*: Quit and retur to previous terminal window <br>
> 
> #### Other commands:
> - **whoami**
> returns the username of the current user

> ### Standard FHS directories
> Directly below the root directory, you’ll find standard FHS directories. 
> 
> **/home:** Each user in the system gets their own home directory. <br>
>
> **/bin:** This directory stands for “binary” and contains binary files and other executables. Executables are files that contain a series of commands a computer needs to follow to run programs and perform other functions. 
>
> **/etc:** This directory stores the system’s configuration files.
>
> **/tmp:** This directory stores many temporary files. The /tmp directory is commonly used by attackers because anyone in the system can modify data in these files.
>
> **/mnt:** This directory stands for “mount” and stores media, such as USB drives and hard drives.

> **<u>TIP:</u>** You can use the man ``hier command`` to learn more about the FHS and its standard directories