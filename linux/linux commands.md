### Hardware Information Commands

| Command                 | Description                                                        |
|-------------------------|--------------------------------------------------------------------|
| lscpu                   | See CPU information.                                               |
| lsblk                   | See information about block devices.                                |
| lspci -tv               | Show PCI devices in a tree-like diagram.                            |
| lsusb -tv               | Display USB devices in a tree-like diagram.                         |
| lshw                    | List hardware configuration information.                             |
| cat /proc/cpuinfo       | Show detailed CPU information.                                      |
| cat /proc/meminfo       | View detailed system memory information.                            |
| cat /proc/mounts        | See mounted file systems.                                           |
| free -h                 | Display free and used memory.                                       |
| sudo dmidecode          | Show hardware information from the BIOS.                            |
| hdparm -i /dev/[device] | Display disk data information.                                      |
| hdparm -tT /dev/[device]| Conduct a read speed test on the device/disk.                       |
| badblocks -s /dev/[dev] | Test for unreadable blocks on the device/disk.                      |
| fsck /dev/[device]      | Run a disk check on an unmounted disk or partition.                 |

### Searching Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| find [path] -name [pattern]       | Find files and directories by pattern in a specified location.      |
| find [path] -size [+100M]         | See files and directories larger than a specified size.             |
| grep [pattern] [file_name]        | Search for a specific pattern in a file.                            |
| grep -r [pattern] [directory]     | Recursively search for a pattern in a directory.                     |
| locate [name]                     | Locate all files and directories related to a particular name.      |
| which [command]                   | Search the command path in the $PATH environment variable.          |
| whereis [command]                 | Find the source, binary, and manual page for a command.             |
| awk '[pattern] {print $0}' [file] | Print all lines matching a pattern in a file.                        |
| sed 's/[old]/[new]/' [file]       | Find and replace text in a file.                                     |

### File Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| mkdir [directory_name]            | Create a new directory.                                             |
| rm [file_name]                    | Remove a file.                                                      |
| rm -r [directory_name]            | Remove a directory recursively.                                      |
| cp [source] [destination]         | Copy contents of one file to another.                                |
| mv [source] [destination]         | Move or rename files or directories.                                 |
| ln -s [path]/[file] [link_name]   | Create a symbolic link to a file.                                    |
| touch [file_name]                 | Create a new file.                                                   |
| cat [file_name]                   | Show the contents of a file.                                         |
| head [file_name]                  | Show the first ten lines of a file.                                  |
| tail [file_name]                  | Show the last ten lines of a file.                                   |
| nano [file_name]                  | Open or create a file using the nano text editor.                    |
| vi/vim [file_name]                | Open or create a file using the Vi/Vim text editor.                   |
| gpg -c [file_name]                | Encrypt a file.                                                      |
| wc -w [file_name]                 | Show the number of words in a file.                                  |

### Directory Navigation Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| ls                                | List files and directories.                                         |
| ls -a                             | List all files and directories (including hidden ones).             |
| ls -l                             | List files and directories in long format.                           |
| pwd                               | Show the current directory.                                          |
| cd                                | Change to home directory.                                            |
| cd ..                             | Move up one directory level.                                         |
| cd -                              | Change to the previous directory.                                    |
| mkdir [directory_name]            | Create a new directory.                                              |
| rmdir [directory_name]            | Remove an empty directory.                                           |
| cp -r [source] [destination]      | Recursively copy a directory.                                        |
| mv [source] [destination]         | Move or rename files or directories.                                 |
| ln -s [path]/[file] [link_name]   | Create a symbolic link to a file.                                    |

### File Compression Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| tar cf [archive.tar] [file/dir]   | Archive a file or directory.                                        |
| tar xf [archive.tar]              | Extract an archived file.                                           |
| tar czf [archive.tar.gz]          | Create a .gz compressed tar archive.                                |
| gzip [file_name]                  | Compress a file with .gz extension.                                 |
| gunzip [file_name.gz]             | Decompress a .gz file.                                              |
| bzip2 [file_name]                 | Compress a file with .bz2 extension.                                |
| bunzip2 [file_name.bz2]           | Decompress a .bz2 file.                                             |

### File Transfer Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| scp [source] [user]@[remote]:[dest] | Securely copy files to/from a remote server.                       |
| rsync -a [source] [user]@[remote]:[dest] | Synchronize directories with a remote backup.                    |
| wget [link]                       | Download files from web servers.                                    |
| curl -O [link]                    | Transfer data to/from a server using various protocols.            |
| ftp [remote_host]                 | Transfer files between local and remote systems using FTP.          |
| sftp [user]@[remote_host]         | Securely transfer files between hosts using SFTP.                    |

### User and Group Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| sudo useradd [user_name]          | Create a new user.                                                  |
| sudo userdel [user_name]          | Delete a user.                                                       |
| sudo passwd [user_name]           | Change user password.                                               |
| sudo groupadd [group_name]        | Create a new group.                                                 |
| sudo groupdel [group_name]        | Delete a group.                                                       |
| sudo usermod -aG [group_name] [user_name] | Add a user to a group.                                          |
| chown [user_name] [file/dir]      | Change file/directory ownership.                                    |
| chgrp [group_name] [file/dir]     | Change file/directory group ownership.                              |
| id                                | Display user and group IDs.                                          |
| last                              | Show last system logins.                                             |

### Package Installation Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| sudo apt-get install [pkg_name]   | Install a package using APT.                                         |
| sudo apt search [keyword]         | Search for packages in APT repositories.                             |
| sudo apt show [pkg_name]          | Show information about a package.                                    |
| sudo dpkg -i [pkg_name.deb]       | Install a .deb package using dpkg.                                   |
| sudo yum install [pkg_name]       | Install a package using YUM.                                         |
| yum search [keyword]              | Search for packages in YUM repositories.                             |
| sudo dnf install [pkg_name]       | Install a package using DNF.                                         |
| sudo rpm -i [pkg_name.rpm]        | Install a .rpm package using rpm.                                    |
| sudo snap install [pkg_name]      | Install a Snap package.                                               |
| flatpak install [pkg_name]        | Install a Flatpak package.                                           |
| make                              | Compile and install software from source code.                         |

### Process Related Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| ps                                | List active processes.                                               |
| top                               | Display all running processes.                                       |
| kill [process_id]                 | Terminate a process by ID.                                           |
| pkill [process_name]              | Terminate a process by name.                                         |
| killall [label]                   | Terminate all processes with a label.                                |
| pstree                            | Show processes in a tree-like diagram.                               |
| pmap                              | Display a memory usage map of processes.                             |
| bg                                | List and resume stopped jobs in the background.                       |
| fg                                | Bring the most recently suspended job to the foreground.             |
| lsof [file]                       | List files opened by running processes.                             |
| nohup [command] &                 | Run a process in the background.                                      |

### System Management and Information Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| uname -a                          | Display system information.                                         |
| uptime                            | Show system uptime and load average.                                |
| hostname                          | Display system hostname.                                            |
| last reboot                       | List system reboot history.                                         |
| date                              | Show current time and date.                                         |
| timedatectl                       | Query and change system clock settings.                             |
| cal                               | Show current calendar.                                              |
| w                                 | Display who is logged in and their activity.                         |
| whoami                            | Display current user.                                                |
| finger [user]                     | Show information about a user.                                      |
| modprobe [module_name]            | Add a new kernel module.                                            |
| dmesg                             | Show bootup messages.                                               |
| shutdown [time]                   | Schedule a system shutdown.                                          |

### Disk Usage Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| df -h                             | Check free and used space on mounted systems.                       |
| df -i                             | Show free inodes on mounted file systems.                          |
| fdisk -l                          | Display disk partitions, sizes, and types.                          |
| du -sh                            | Show disk usage of the current directory.                           |
| mount                             | Show currently mounted file systems.                                 |
| findmnt                           | Display target mount point for all file systems.                     |


### SSH Login Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| ssh [user_name]@[remote_host]     | Connect to a remote host via SSH.                                   |
| ssh -p [port] [user_name]@[remote_host] | Connect to a host using a specific port.                        |
| ssh-keygen                        | Generate SSH key pairs.                                             |
| scp [file_name] [user_name]@[remote_host]:[remote_path] | Securely copy files using SSH. |
| sftp [user_name]@[remote_host]    | Securely transfer files using SFTP.                                  |
| telnet [host]                     | Connect to a host via Telnet.                                       |

### File Permission Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| chmod [permissions] [file_name]   | Change file permissions.                                            |
| chown [user_name] [file_name]     | Change file ownership.                                              |
| chgrp [group_name] [file_name]    | Change file group ownership.                                         |
| umask [mode]                      | Set default permissions for new files.                               |

### Network Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| ip addr show                      | List IP addresses and network interfaces.                            |
| ifconfig                          | Display IP addresses of all network interfaces.                     |
| ping [remote_host]                | Ping a remote host.                                                 |
| netstat -pnltu                    | List active (listening) ports.                                       |
| nslookup [domain_name]            | Look up IP address for a domain.                                     |
| dig [domain_name]                 | Show DNS information for a domain.                                   |

### Variable Commands

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| export [variable_name]=[value]    | Export a shell variable.                                            |
| declare -x [variable_name]=[value]| Declare and export a shell variable.                                |
| unset [variable_name]             | Unset a shell variable.                                             |
| echo $[variable_name]             | Display the value of a shell variable.                               |
| set                               | Display all shell variables.                                         |

### Shell Command Management

| Command                           | Description                                                        |
|-----------------------------------|--------------------------------------------------------------------|
| alias [alias_name]='[command]'    | Create an alias for a command.                                       |
| unalias [alias_name]              | Remove an alias.                                                     |
| history                           | Display command history.                                             |
| man [command]                     | Display manual for a command.                                        |
| which [command]                   | Show location of a command.                                          |
| type [command]                    | Display command type.                                                |
| whereis [command]                 | Find location of a command.                                          |
| locate [file_name]                | Search for a file.                                                   |

### Linux Shell Keyboard Shortcuts

| Shortcut                           | Description                                                       |
|------------------------------------|--------------------------------------------------------------------|
| Ctrl + C                           | Kill the current process.                                          |
| Ctrl + Z                           | Suspend the current process.                                       |
| Ctrl + D                           | Logout from the current session.                                   |
| Ctrl + W                           | Cut the word before the cursor.                                    |
| Ctrl + U                           | Cut the line before the cursor.                                    |
| Ctrl + K                           | Cut the line after the cursor.                                     |
| Ctrl + Y                           | Paste from clipboard.                                              |
| Ctrl + R                           | Search command history.                                            |
| Ctrl + O                           | Run the previous command.                                          |
| Ctrl + G                           | Exit command history without running a command.                    |
| Ctrl + L                           | Clear the screen.                                                  |
| Ctrl + A                           | Move to the beginning of the line.                                 |
| Ctrl + E                           | Move to the end of the line.                                       |
| Ctrl + P                           | Move to the previous command in history.                           |
| Ctrl + N                           | Move to the next command in history.                               |
| Ctrl + T                           | Swap the last two characters before the cursor.                    |
| Ctrl + X + Ctrl + E                | Open an editor to run a command.                                   |
| Ctrl + H                           | Delete the character before the cursor.                            |
| Ctrl + D                           | Delete the character under the cursor.                             |
| Ctrl + R                           | Search command history interactively.                              |
| Ctrl + Z                           | Suspend the current foreground process.                           |
| Ctrl + \                           | Quit the current process.                                          |
