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

> #### Standard FHS directories
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

> **<u>TIP:</u>** You can use the ``hier`` command to learn more about the FHS and its standard directories

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

> ### Filtering commands
>
> - **grep**
> Searches a specified file and returns all lines in the file containing a specified string. <br>
> Syntax: `grep <string> <file_name>` <br>
> Example: `grep OS updates.txt`
>
> - **|**(piping)
> Sends the standard output of one command as the standard input to another command for further processing <br>
> Syntax: ` <first_command> | <second_command>` <br>
> Example: `ls home/analyst/reports | grep users`
>
> - **find**
> searches for directories and files that meet specified criteria <br>
> The criteria can be:
>>> - Contain a specific string in the name,
>>> - Are a certain file size, or
>>> - Were last modified within a certain time frame. <br>
> Syntax: `find <directory|location_to_search> <criteria>` <br>
>
> *Note: if you don't include a criteria, it will likely return alot of directories and files*
>
>> Specifying criteria involves options. **Options** modify the behaviour of a command and commonly begin with a hyphen (`-`). <br>
>> **-name and -iname** <br>
>> These are used to  find file or directory names that contain a specific string. The difference between these two options is that `-name` is case-sensitive, and `-iname` is not. 
>> The specific string you’re searching for must be entered in quotes after the `-name` or `-iname` options. <br>
> Examples: <br>  `find /home/analyst/projects -name "*log*"` <br> `find /home/analyst/projects -iname "*log*"`
>
>>_Note: An asterisk (*) is used as a wildcard to represent zero or more unknown characters._
>
>> **-mtime** <br>
>> This criteria is used when the analyst wants to find files or directories that were modiefied within certain time frame. <br>
>> The `-mtime` option search is based on days.
> Syntax:
> Examples: <br> `find /home/analyst/projects -mtime -1` <br>
`find /home/analyst/projects -mtime +1` <br>
> where `+1` indicates all files/directories last modified more than one day ago and `-1` indicates all files/directories modified less than one day ago
>
>> ___Note__: The option `-mmin` can be used instead of `-mtime` if you want to base the search on minutes rather than days._

> ### Creating and modifying files/directoris commands
>
> - **mkdir** <br>
> Creates a new directory <br>
> Syntax: `mkdir <directory_name>` <br>
> Example: `mkdir home` <br>
>
> - **rmdir** <br>
> Removes a directory. (opposite of mkdir) <br>
> Syntax: `rmdir <directory_name>` <br>
> Example: `rmdir home` <br>
>
> - **touch** <br>
> Creates a new file <br>
> Syntax: `touch <file_name_with_extension>` <br>
> Example: `touch data.txt` <br>
>
> - **rm** <br>
> Removes or deletes a file
> Syntax: `rm <file_name_with_extension>` <br>
> Example: `rm data.txt` <br>
>
> - **mv** <br>
> Moves a file/directory to new location.  <br>
> _Note: You must be in directory of the file to move._ <br>
> Syntax: `mv <file_name_with_extension> <location_to_move>` <br>
> Example: `mv project_info.txt /home/analyst/data` <br>
>
> - **cp** <br>
> Copies a file or directory into a new location <br>
> _Note: You must be in directory of the file to copy._ <br>
> Syntax: `cp <file_name_with_extension> <location_to_copy>` <br>
> Example: `cp projects.txt /home/analyst/project` <br>
>
> _**Note**: Use `ls` to check for changes_
>
> - **nano** <br>
> Nano is a text editor, using nano command will edit the file using text editor. <br>
> Syntax: `nano <file_name_with_extension>` <br>
> Example: `nano OS_patches.txt` <br>
> Editor shortcuts: <br>
> `CTRL + O` -> save
> `Enter` -> save with current file name
> `CTRL + X` -> exit
>
>> ### Standard output redirection
>> In addition to the pipe (|), you can also use the right angle bracket (>) and double right angle bracket (>>) operators to redirect standard output. <br>
>> The difference between the two is that `>` overwrites your existing file, and `>>` adds your content to the end of the existing file instead of overwriting it. The > operator should be used carefully, because it’s not easy to recover overwritten files. <br><br>
>> *Examples:* <br>
>> While in a directory containing `permissions.txt`, <br>
>> -- entering `echo "last updated date" >> permissions.txt` adds the string _"last updated date"_ to the file content. <br>
>> -- Entering `echo "time" > permissions.txt` overwrites the entire file contents of `permissions.txt` with the string _“time”_.

## File and Directory permissions

> #### Permissions
> The type of access granted for a file or directory
>
> #### Authorization
> The concept of granting access to specific resources in a system
>
> ### Permissions in Linux
> - read (r)
> - write (w)
> - execute (x)
> 
> _Permissions are granted to three different types of owners. They are:_ <br> 
> - Users (u) <br>
> Owner of the file (the user who creates the file is owner by default, but it can be changed) <br>
> - Group (g) <br>
> Every user is part of a group. Group is a number of users together. <br>
> - Other (o) <br>
> All other users on the system <br>
>
> Example of how a file with all permissions looks like: <br>
> `drwxrwxrwx` <br>
> where <br>
> `d` - says its a directory, else files have `-` <br>
> `rwx` [2nd,3rd,4th characters] - says the first type of owner (user) has read(r),write(w),execute(x) permissions <br>
> `rwx` [5th,6th,7th characters] - says the second type of owner (group) has read(r),write(w),execute(x) permissions <br>
> `rwx` [8th,9th,10th characters] - says the third type of owner (other) has read(r),write(w),execute(x) permissions <br>
> If any permission is not allowed, the option is replaced with `-` <br>
>> For example: *-rwxrw-r--* <br> Here, the permissions are for a file, with user having read, write, execute, group having read,write and other having only read permissions <br>
> ![permissions_rwx](image-7.png)
> 
> ## Checking permissions 
> #### Options
> Modify the behavior of the command
>
> ## Permission checking commands
> **`ls -l`** <br>
> displays permissions to files and directories <br>
>
> **`ls -a`** <br>
> displays hidden files <br>
>
> **`ls -la`** <br>
> Combination of previous two commands ~ displays permissions to files and directories including hidden files <br>
>
> ## Changing Permissions
>  
> **chmod** <br> 
> Changes permissions for files and directories. "chmod" is short for changemode. The chmod command requires two arguments. The first argument indicates how to change permissions, and the second argument indicates the file or directory that you want to change permissions for.   <br> 
> 
>  <br> <br>
> Syntax: `chmod <owner_type><+/-><permission>, <owner_type2><+/-><permission>, <owner_type3><+/-><permission> <file>` <br>
> `+` indicates "add" <br>
> `-` indicated "remove" <br>
> Example: `chmod g+w, o-r access.txt`<br>
> Here, we are changing permissions to enable *group* to write (`g+w`) and remove *other*'s read(`o-r`) permission for the file *access.txt*
> <br>
> 
> ![characters_in_chmod](image-8.png)

> ## User Commands
>
> ### Root User (or Superuser)
> A user with elevated privileges to modify the system.
>
> # Problems iwth logging in as root
> - Security risk
> - Easy to make irreversible mistakes
> - Accountability
> 
> One of the solutions for this is the use of: <br>
> **`sudo`** (super-user do) <br>
> Temporarily grants elevated permissions to specific users. Users must be given access in a configuration file to use `sudo`. The file is called the "sudoers file". <br>
>
> **`useradd`**<br>
> Adds a user to the system. This can only be used by root user or sudo user. <br>
> Example: <br>
> To add a user with the username of fgarcia with sudo, enter `sudo useradd fgarcia`. There are additional options you can use with useradd:
>
>>`-g`: Sets the user’s default group, also called their primary group
>
>>`-G`: Adds the user to additional groups, also called supplemental or secondary groups
>
>To use the `-g` option, the primary group must be specified after `-g`. For example, entering `sudo useradd -g security fgarcia` _adds fgarcia as a new user and assigns their primary group to be security._
>
> To use the `-G` option, the supplemental group must be passed into the command after `-G`. _You can add more than one supplemental group at a time with the -G option._ Entering `sudo useradd -G finance,admin fgarcia` adds _fgarcia_ as a new user and adds them to the existing finance and admin groups. <br>
>
>**`usermod`** <br>
>The `usermod` command modifies existing user accounts. The same `-g` and `-G` options from the `useradd` command can be used with `usermod` <u> if a user already exists. </u> <br>
>
>To change the primary group of an existing user, you need the `-g`option. For example, entering `sudo usermod -g executive fgarcia` would change fgarcia’s primary group to the executive group. <br>
>
>To add a supplemental group for an existing user, you need the `-G` option. You also need a `-a` option, which appends the user to an existing group and is only used with the `-G` option. <br> For example, entering `sudo usermod -a -G marketing fgarcia` would add the existing fgarcia user to the supplemental marketing group. <br>
>
>> _**Note**: When changing the supplemental group of an existing user, if you don't include the `-a` option, `-G` will replace any existing supplemental groups with the groups specified after usermod.  Using `-a` with `-G` ensures that the new groups are added but existing groups are not replaced._ <br>
>
> There are other options you can use with usermod to specify how you want to modify the user, including: <br>
>
>`-d`: Changes the user’s home directory. <br>
>
>`-l`: Changes the user’s login name. <br>
>
>`-L`: Locks the account so the user can’t log in. <br>
>
> The option always goes after the usermod command. For example, to change fgarcia’s home directory to `/home/garcia_f`, enter `sudo usermod -d /home/garcia_f fgarcia`. The option `-d` directly follows the command `usermod` before the other two needed arguments.
>
>**`userdel`** <br>
> Deletes a user from the system. This requires root user previleges as well. <br>
> Example:  entering `sudo userdel fgarcia` deletes fgarcia as a user. <br>
> The `userdel` command doesn’t delete the files in the user’s home directory unless you use the -r option. Entering `sudo userdel -r fgarcia` would delete fgarcia as a user and delete all files in their home directory. Before deleting any user files, you should ensure you have backups in case you need them later. <br>
>
>> _**Note**: Instead of deleting the user, you could consider deactivating their account with usermod -L. This prevents the user from logging in while still giving you access to their account and associated permissions._
> <br>
>
> **`chown`** <br>
> The chown command changes ownership of a file or directory. You can use chown to change user or group ownership. <br>
> For example: To change the _user owner_ of the _access.txt_ file to fgarcia, enter `sudo chown fgarcia access.txt.` To change the _group owner_ of access.txt to security, enter `sudo chown :security access.txt`. You must enter a colon (:) before security to designate it as a group name. <br> 
>
> - Similar to useradd, usermod, and userdel, there are additional options that can be used with chown.

> ## Resources available in the shell
> Linux has built-in commands for support/information. <br>
>
> **`man`**: (short for manual)<br>
> This command displays information on other commands and how they work.
> <br>
>**`whatis`**: <br>
> Displays a description of a command on a single line <br>
>
> **`apropos`**: <br>
> Searches the manual page decription for a specified string <br>



# Module 4 **Databases & SQL**
>
> ## Databases
> An organized collection of information or data <br>
> - Accessed by multiple people simultaneously
> - Store massive amounts of data
> - Perform complex tasks while accessing data
>
> ## Relational database
> A structured database containing tables that are related to each other <br>
> ## Primary key
> A column where every row has a unique entry
>
> ## Foregin key
> A column in a table that is primary key in another table
>
>> _**Note**: A table can have one primary key but multiple foregin keys_
>
> ## SQL (Structured Query Language)
> A programming language used to create, interact with, and request information from a database.
>
> ### Query
> A request for daata from a tabase table or a combination of tables
>
> ### Log 
> A record of event that occurs within an organisation's systems
>
> ## Accessing SQL in Linux
> To access SQL from Linux, you need to type in a command for the version of SQL that you want to use. For example, if you want to access SQLite, you can enter the command `sqlite3` in the command line.

> ## SQL Queries
> 
> #### Syntax
> The rules that determine whaat is correctly structured in a computing language <br>
>
> ### SQL Keywords
>
> **SELECT** <br>
> Indicates which columns to return <br>
>  <br>
> 
> **FROM** <br>
> Indicates which table to query. The `SELECT` keyword always comes with the `FROM` keyword.  <br>
>
> Syntax: `SELECT <column_name> FROM <table_name>;` <br>
> Example: `SELECT employee_id, device_id FROM employees;`<br>
> This displays the employee_id and device_id rows from the table "employees'. <br>
>
>> _**Note**: `*` refers to all the data in the table (in this case)_
>
> **ORDER BY** <br>
> `ORDER BY` sequences the records returned by a query based on a specified column or columns. This can be in either ascending or descending order. <br>
> 
> Syntax: `SELECT <column_name> FROM <table_name> ORDER BY <column_name;` <br>
> Example: `SELECT customerid, city, country FROM customers ORDER BY city;` <br>
> This will return the _customerid, city, and country_ columns from the _customers_ table, and the records will be sequenced by the _city_ column. <br>
>
> The `ORDER BY` keyword sorts the records based on the column specified after this keyword. By default, as shown in this example, the sequence will be in ascending order. This means:
> - if you choose a column containing numeric data, it sorts the output from the smallest to largest. For example, if sorting on customerid, the ID numbers are sorted from smallest to largest.
> - if the column contains alphabetic characters, such as in the example with the city column, it orders the records from the beginning of the alphabet to the end.
>
> ### Sorting in descending order
>
> To sort in descending order, we use the keyword `DESC` after mentioning the column after `ORDER BY`.
>
> For example: <br>
> `SELECT customerid, city, country FROM customers ORDER BY city DESC;`
>
> ### Sorting based on multiple columns
> Sorting can be done with multiple columns as well. <br>
> For example, you might first choose the _country_ and then the _city_ column. SQL then sorts the output by country, and for rows with the same country, it sorts them based on city. 
> Query example: `SELECT customerid, city, country FROM customers ORDER BY country, city;`
>
>
> ## Filtering
> Selecting data that matche a certain condition
>
> #### Operator
> a symbol or keyword taht represents an operation 
>
> **WHERE**
> indicates a condition for a filter. After using keyword `WHERE` the condition is listed using operators. <br>
> Example: `SELECT customerid, city, country FROM customers WHERE country = 'USA';` <br>
>
>
> ### Filtering for patterns
> Filtering can also be done based on patterns, ot requires two elements:
> - a wildcard
> - the `LIKE` operator
>
> - **Wildcards**
>A wildcard is a special character that can be substituted with any other character. Two of the most useful wildcards are the percentage sign (%) and the underscore (_):
>> - The percentage sign substitutes for any number of other characters. 
>> - The underscore symbol only substitutes for one other character. <br>
> These wildcards can be placed after a string, before a string, or in both locations depending on the pattern you’re filtering for. <br>
> The following table includes these wildcards applied to the string 'a' and examples of what each pattern would return. <br>
> ![wildcards_patterns](image-9.png)
><br>
> - **The `LIKE` Operator** <br>
> To apply wildcards to the filter, you need to use the LIKE operator instead of an equals sign (=). LIKE is used with WHERE to search for a pattern in a column.  <br>
>For instance, if you want to email employees with a title of either 'IT Staff' or 'IT Manager', you can use LIKE operator combined with the % wildcard:  <br>
> Query: `SELECT lastname, firstname, title, email FROM employees WHERE title LIKE 'IT%';` <br>
> This query returns all records with values in the title column that start with the pattern of 'IT'. This means both 'IT Staff' and 'IT Manager' are returned. <br>
> 
> As another example, if you want to search through the invoices table to find all customers located in states with an abbreviation of 'NY', 'NV', 'NS' or 'NT', you can use the 'N_' pattern on the state column: <br>
> Query: `SELECT firstname,lastname, state, country FROM customers WHERE state LIKE 'N_';`
> <br>
> This returns all the records with state abbreviations that follow this pattern.

> ## Common Data types in Databases
>
> - ### String
> Data consisting of ordered sequence of characters. They could be numbers, letters or symbols.
>
> - ### Numeric
> Data consisting of numbers. Unlike string, mathematical symbols can be used on numeric data.
>
> - ### Date and Time 
> Data representing date and/or time.
>
> #### Operators used with Numeric and Date and time data types
> ![comparison_operators](image-10.png)
_>> **Note**: You can also use != as an alternative operator for not equal to._ <br>
>
> **BETWEEN** <br>
> An operator that filters for numbers or dates within a range <br>
> Syntax: `.... BETWEEN <beginning_of_range> AND <end_of_range>;` <br>
>> _**Note**: Numberical data types don't need quotaion marks_ <br>
>
><br>
> 
> ### Logical Operators
> **AND** <br>
> Specifies that both conditions must be met simultaneously <br>
>
> **OR** <br>
> Specifies that either condition can be met <br>
>
> **NOT** <br>
> Negates a condition <br>
>
> Logical operators can be combined in filters. For example, if you know that both the USA and Canada are not affected by a cybersecurity issue, you can combine operators to return customers in all countries besides these two. In the following query, NOT is placed before the first condition, it's joined to a second condition with AND, and then NOT is also placed before that second condition. <br>
> Example Query: `SELECT firstname, lastname, email, country FROM customers WHERE NOT country = 'Canada' AND NOT country = 'USA';` <br>
>
>> _**Pro tip**: Another way of finding values that are not equal to a certain value is by using the <> operator or the != operator. For example, WHERE country <> 'USA' and WHERE country != 'USA' are the same filters as WHERE NOT country = 'USA'._

> ## Joining Tables in Database
>
> **INNER JOIN** <br>
>  Returns rows matching on a specific column that exists in more than one table. <br>
> ![inner_join](image-11.png) <br>
>
> Syntax: `SELECT <table1_columns> FROM <table1> INNER JOIN <table_2> ON <table1>.<matching_column> = <table2>.<matching_column>`<br>
> Example: `SELECT * FROM employees INNER JOIN machines ON employees.device_id = machines.device_id;` <br>
>
> **OUTER JOIN** <br>
>
>  Has three types: <br>
>
> - LEFT JOIN <br>
> Returns all the records of the first table, but only returns rows of the second table that match on a specified column <br>
> ![left_join](image-12.png)
> > Syntax: `SELECT <table1_columns> FROM <table1> LEFT JOIN <table_2> ON <table1>.<matching_column> = <table2>.<matching_column>`<br>
> - RIGHT JOIN <br>
> Returns all the records of the second table, but only returns the rows from the first table that match on specified column 
> ![right_join](image-13.png)
> > Syntax: `SELECT <table1_columns> FROM <table1> RIGHT JOIN <table_2> ON <table1>.<matching_column> = <table2>.<matching_column>`<br>
> - FULL OUTER JOIN <br>
> Returns all records from both tables
> ![full_join](image-14.png)
> > Syntax: `SELECT <table1_columns> FROM <table1> FULL OUTER JOIN <table_2> ON <table1>.<matching_column> = <table2>.<matching_column>`<br>

> ## Aggregate Funcitons
> These are functions that perform a calculation over multiple data points and return the result of the calculation. The actual data is not returned. 
>
>There are various aggregate functions that perform different calculations:
>
> - **COUNT**: <br> returns a single number that represents the number of rows returned from your query. <br>
>
> - **AVG**: <br> returns a single number that represents the average of the numerical data in a column. <br>
>
> - **SUM**: <br> returns a single number that represents the sum of the numerical data in a column. <br>
>