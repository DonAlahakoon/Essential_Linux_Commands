# Essential_Linux_Commands
![Picture](https://opencode.md/wp-content/uploads/2023/08/Top-8-facts-about-Linux-2.jpg)
## *** This repository contains some of the important often used Linux commands anyone interested in learning Linux should know. ***
> [!TIP]
>  Hint✨: To search 🔎 any command or any operation use <i>Ctrl + F</i>
## 1. ssh
> ``` ssh <username>@<serverIP>```
## 2. ls
 List all the files in the directory<br>
> ```ls -l``` gives list files with permissions<br>
> ```ls -al``` gives hidden files as well<br>
## 3. pwd
 Be able to print the current directory
## 4. cd
 Changing directory<br>
> ```cd /<path>```   navigate to the respective directory<br>
> ```cd ..  ```      jump back directory<br>
> ```cd   ```        naviagate to home
## 5. touch
> ```touch <filename> ``` create a new file<br>
> ```touch <filename1> <filename2> ``` create several files<br>
> ```touch <filename>{1..10} ```create 10 files

## 6. echo
> ```echo <message>```  print the message<br>
> ```echo <message>  > <filename>``` Add message in to the file<br>


## 7. nano
> ```nano <filename>``` edit a file<br>
> To save use ctrl + X then Y then Enter to save

> [!TIP]
> To undo use "Alt + U" and to redo "Alt + E"
## 8. vim
> ```vim <filename>``` edit a file<br>
> Hit I to start editing
> When done use hit ESC and :wq 
## 9. cat
> ```cat <filename>``` Read content of a file<br>

> [!TIP]
> To find the OS version use ```cat /etc/os-release```
## 10. shred
> ```shred <filename>``` Don't let anyone to read the file. 
## 11. mkdir
> ```mkdir <directory name>``` create a new directory
## 12. cp
> ```cp <file name> <path where to copy>``` Copy file to a given path
> ```mv <file name> \<path where to move>``` Move file to the given path 
## 13. rm
> ```rm <file name>``` Remove a file
## 14. rmdir
> ```rmdir <directory name>``` For an empty directory removal<br>
> ```rm -r <directory name>``` To remove a directory with files in it
## 15. ln
> ```ln -s <file name> <link>``` Can create a link to a file with -s switch for soft
## 16. clear
 Clear the terminal
## 17. whoami
 Tells who you are😄 (returns the username)
## 18. useradd
> ```useradd <name>``` Create a new user
## 19. sudo
> ```sudo <command which needs permission>``` Uses when asked for permission
> Need to enter the password for user
## 20. adduser
Can reverse the command useradd
## 21. su
>```su <username>``` Can switch user
## 22. exit 
 Exit temparary user. (can use in several occasions)
## 23. passwd
> ```passwd <username>``` Can change the password of the user
## 24. apt
> ```sudo apt update``` Needs to update before install for Debian based Linux distributions (For other distros yum)
> ```sudo apt install <package>``` Install packages
## 25. finger
 Needs to install finger package first
> ```finger  <username>``` Can be used to inspect another user
## 26. man
> ```man <command>``` Can get help with things that don't know
## 27. whatis 
> ```whatis <command>``` Faster than man command to get help
## 28. whereis
> ```whereis <command>``` To findout where the command is 
## 29. wget
> ```wget <link>``` Help to get stuff from the internet (download)
## 30. curl
> ```curl <link>``` Help to get stuff from the internet
## 31. zip
> ```zip <zip file> <file name>``` Make a zip file
## 32. unzip
> ```unzip <zip file name>``` Unzip the file
## 33. less
>```less <file name>``` Can read one page at a time. (substitution for cat command)
## 34. head
>```head <file name>``` Output only the begining of the file
## 35. tail
>```tail <file name>``` Output only the ending of the file
## 36. cmp
>```cmp <file1> <file2>``` Compare two files and check whether any differences exist.
## 37. diff
>```diff <file1> <file2>``` List the differences of the two files
## 38. sort
>```cat <file name> | sort``` The file is sorted in alphabatical order
## 39. find
>```sudo find <the directory> -name "<search key>"``` Find the search key<br>
>```sudo find <the directory> -type f -name "."``` Find all hidden files<br>
>```find <the directory> -type f -empty``` Finds all empty directories<br>
>```find <the directory> -perm /a=x``` Finds all executable files<br>
## 40. chmod
Change the permissions of the file
>```chmod <permission> <file name>``` To change permission of the file.

> [!IMPORTANT]
> Here are the permission types<br>
> 0 no permissions<br>
> 1 can execute<br>
> 2 can write<br>
> 3 can write, execute<br>
> 4 can read<br>
> 5 can read, execute<br>
> 6 can read, write<br>
> 7 can read, write and execute<br>

> [!NOTE]
> Symbolic method:<br>
> ```chmod o=rwx <filename>``` Which means overwrite other group permission into rwx<br>
> ```chmod g+x <filename>``` Which means it add execute permission into group<br>
> ```chmod u-r <filename>``` remove read permission from the user<br>
## 41. chown
>```chown <user> <file name>``` Changing owner of the file
## 42. ifconfig
 Gives IP address of the machine
## 43. ip address
 Returns the ip address

> [!NOTE]
> Can also use the command ```grep``` to only return ip address of a specific interface.
> Ex: >```ip address | grep eth0``` Return only the ip address of ethernet 0.

> [!IMPORTANT]
> If only the ip address you want to return, use ```awk '{print $2}' ```<br>
> Ex: >```ip address | grep eth0 | grep inet | awk '{print $2}'```

## 44. resolvectl status
Return information about the DNS server (including IP address)

> [!TIP]
> ```cat /etc/resolv.conf``` Return information about the DNS server
## 45. ping
> ```ping <name of the website/ipaddress>```

> [!TIP]
> Use ctrl+C to stop.

> [!NOTE]
> To use only a specific number of response use ```ping -c <number> <name of the website/ipaddress>```<br>
> To use only a specific size of packets use ```ping -s <number> <name of the website/ipaddress>```
## 46. traceroute
>```traceroute <name of the website>```To see the path through the internet to get to a website
## 47. netstat
> To check what ports in use.

> [!TIP]
> Modern version ```netstat -tulpn```<br>
> Another command ```ss``` or ```ss -tulpn```
## 48. iptables
> ```sudo iptables -I INPUT -p tcp -, tcp --dport <port> -j ACCEPT```To allow a specific port through the firewall

> [!TIP]
> Easy command ```sudo ufw allow <port>```

> [!IMPORTANT]
> To execute above command below command might need to execute first<br>
> ```sudo ufw enable```
> To check status use ```sudo ufw status```
## 49. uname
>```uname -a``` To find information about the system.

> [!NOTE]
> Use ```lsb_release```  to find information about Linux distribution version

> [!TIP]
> Needs prettier version than above😀<br>
> Install neofetch ```sudo apt install neofetchf```<br>
> Run```neofetch```
## 50. cal
 A quick little calendar :)
## 51. free
 To check how much memeory available in system and <b>swap<b> space.
> [!NOTE]
> Here swap means the virtual memory. Once the RAM is fully utilize OS uses secondary memory to create a virtual memory. 
## 52. df
 To check how much space available (To be more specific use df -H)
## 53. ps
 To list all processes<br>
> ```ps -aux``` More details
## 54. top
 List processes running in real time

> [!TIP]
> ```htop``` Much more prettier version of top. 
## 55. kill
>```kill -KILL <pid>``` or ```kill -9 <pid>``` To kill the process with given id.

> [!TIP]
> Use ```pkill -f <name of the process>``` In case the pid is not known.
## 56. systemctl
>```systemctl stop <service name>``` Stop a specific service.<br>
>```systemctl start <service name>``` Start a specific service.<br>
>```systemctl restart <service name>``` Restart a specific service<br>

> [!TIP]
>```systemctl status <service name>``` To check the status<br>
> Use ```sudo``` if necessary when using ```systemctl``` command
## 57. history
Return a list of commands used.
## 58. reboot
>```sudo reboot``` To reboot the system
## 59. shutdown
>```sudo shutdown``` To shutdown the system after 1 minute<br>
>```sudo shutdown -h now``` To shutdown the system now

## 60. stat
>```stat <filename>``` Gives the meta data of the file.
