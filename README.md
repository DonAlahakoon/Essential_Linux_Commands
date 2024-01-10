# Essential_Linux_Commands
This repository contains some of the important often used Linux commands anyone interested in learning Linux should know.
## 1. ssh
> ``` ssh \<username>@\<serverIP>```
## 2. ls
> List all the files in the directory<br>
> ```ls -l``` gives list files with permissions<br>
> ```ls -al``` gives hidden files as well<br>
## 3. pwd
> Be able to print the current directory
## 4. cd
> Changing directory<br>
> ```cd \<path>```   navigate to the respective directory<br>
> ```cd ..  ```      jump back directory<br>
> ```cd   ```        naviagate to home
## 5. touch
> ```touch \<filename> ``` create a new file<br>
> ```touch \<filename1> <filename2> ``` create several files<br>
> ```touch \<filename>{1..10} ```create 10 files

## 6. echo
> ```echo \<message>```  print the message<br>
> ```echo \<message>  \> \<filename>``` Add message to the file<br>
## 7. nano
> ```nano \<filename>``` edit a file<br>
> To save use ctrl + X and Y and Enter to save
## 8. vim
> ```vim \<filename>``` edit a file<br>
> Hit I to start editing
> When done use hit ESC and :wq 
## 9. cat
> ```cat \<filename>``` Read content of a file
## 10. shred
> ```shred \<filename>``` Don't let anyone to read the file. 
## 11. mkdir
> ```mkdir \<directory name>``` create a new directory
## 12. cp
> ```cp \<file name> \<path where to copy>``` Copy file to a given path
> ```mv \<file name> \<path where to move>``` Move file to the given path 
## 13. rm
> ```rm \<file name>``` Remove a file
## 14. rmdir
> ```rmdir \<directory name>``` For an empty directory removal
> ```rm -r \<directory name>``` To remove a directory with files in it
## 15. ln
> ```ln -s \<file name> <link>``` Can create a link to a file with -s switch for soft
## 16. clear
> Clear the terminal
## 17. whoami
> Tells who you are😄 (returns the username)
## 18. useradd
> ```useradd \<name>``` Create a new user
## 19. sudo
> ```sudo \<command which needs permission>``` Uses when asked for permission
> Need to enter the password for user
## 20. adduser
>Can reverse the command useradd
## 21. su
>```su <username>``` Can switch user
## 22. exit 
> exit temparary user. (can use in several occasions)
## 23. passwd
> passwd <username> Can change the password of the user
## 24. apt
> ```sudo apt update``` Needs to update before install
> ```sudo apt install <package>``` Install packages
## 25. finger
> Needs to install finger package first
> ```finger  \<username>``` Can be used to inspect another user
## 26. man
> ```man \<command>``` Can get help with things that don't know
## 27. whatis 
> ```whatis \<command>``` Faster than man command to get help
## 28. whereis
> ```whereis \<command>``` To findout where the command is 
## 29. wget
> ```wget \<link>``` Help to get stuff from the internet (download)
## 30. curl
> ```curl \<link>``` Help to get stuff from the internet
## 31. zip
> ```zip \<zip file> <file name>``` Make a zip file
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
>```sudo find <the directory> -name "<search key>"``` Find the search key
>```sudo find <the directory> -type f -name "."``` Find all hidden files
>```find <the directory> -type f -empty``` Finds all empty directories
>```find <the directory> -perm /a=x``` Finds all executable files
## 40. chmod
Change the permissions of the file
>```chmod <permission> <file name>``` To change permission of the file.

> [!IMPORTANT]
> 0 no permissions<br>
> 1 can execute<br>
> 2 can write<br>
> 3 can write, execute<br>
> 4 can read<br>
> 5 can read, execute<br>
> 6 can read, write<br>
> 7 can read, write and execute<br>
## 41. 
## 42. 
## 43. 
## 44. 
## 45. 
## 46. 
## 47. 
## 48. 
## 49. 
## 5. 


