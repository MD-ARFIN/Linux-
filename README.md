# Linux-


Linux Commands with Examples
The Linux command is a utility of the Linux operating system. All basic and advanced 
tasks can be done by executing commands. The commands are executed on the Linux 
terminal. The terminal is a command-line interface to interact with the system, which 
is similar to the command prompt in the Windows OS. Commands in Linux are casesensitive.
Linux
provides a powerful command-line interface compared to other operating systems such as Windows
and MacOS. We can do basic work and advanced work through its terminal. We can do some basic 
tasks such as creating a file, deleting a file, moving a file, and more. In addition, we can also perform 
advanced tasks such as administrative tasks (including package installation, user management), 
networking tasks (ssh connection), security tasks, and many more.
Linux terminal is a user-friendly terminal as it provides various support options. To 
open the Linux terminal, press "CTRL + ALT + T" keys together, and execute a 
command by pressing the 'ENTER' key.
In this topic, we will discuss the top 50 most frequently used Linux commands with 
their examples. These commands are very useful for a beginner and professional both. 
We have divided these commands into following sections so that you can easily 
identify their usage:
o Linux Directory Commands
o Linux File Commands
o Linux File Content Commands
o Linux User Commands
o Linux Filter Commands
o Linux Utility Commands
o Linux Networking Command
Linux Top 50 Commands
The following are the top 50 Linux commands:
Linux Directory Commands
1. pwd Command
The pwd
command is used to display the location of the current working directory.
Syntax:
1. pwd
Output:
2. mkdir Command
The mkdir
command is used to create a new directory under any directory.
Syntax:
1. mkdir <directory name>
Output:
3. rmdir Command
The rmdir
command is used to delete a directory.
Syntax:
1. rmdir <directory name>
Output:
4. ls Command
The ls
command is used to display a list of content of a directory.
Syntax:
1. ls
Output:
5. cd Command
The cd
command is used to change the current directory.
Syntax:
1. cd <directory name>
Output:
Linux File commands
6. touch Command
The touch
command is used to create empty files. We can create multiple empty files by executing it once.
Syntax:
1. touch <file name>
2. touch <file1> <file2> ....
Output:
7. cat Command
The cat
command is a multi-purpose utility in the Linux system. It can be used to create a file, display 
content of the file, copy the content of one file to another file, and more.
Syntax:
1. cat [OPTION]... [FILE]..
To create a file, execute it as follows:
1. cat > <file name>
2. // Enter file content
Press "CTRL+ D" keys to save the file. To display the content of the file, execute it as 
follows:
1. cat <file name>
Output:
8. rm Command
The rm
command is used to remove a file.
Syntax:
rm <file name>
Output:
9. cp Command
The cp
command is used to copy a file or directory.
Syntax:
To copy in the same directory:
1. cp <existing file name> <new file name>
To copy in a different directory:
Output:
10. mv Command
The mv
command is used to move a file or a directory form one location to another location.
Syntax:
1. mv <file name> <directory path>
Output:
11. rename Command
The rename
command is used to rename files. It is useful for renaming a large group of files.
Syntax:
1. rename 's/old-name/new-name/' files
For example, to convert all the text files into pdf files, execute the below command:
1. rename 's/\.txt$/\.pdf/' *.txt
Output:
Linux File Content Commands
12. head Command
The head
command is used to display the content of a file. It displays the first 10 lines of a file.
Syntax:
1. head <file name>
Output:
13. tail Command
The tail
command is similar to the head command. The difference between both commands is that it 
displays the last ten lines of the file content. It is useful for reading the error message.
Syntax:
1. tail <file name>
Output:
14. tac Command
The tac
command is the reverse of cat command, as its name specified. It displays the file content in reverse 
order (from the last line).
Syntax:
1. tac <file name>
Output:
15. more command
The more
command is quite similar to the cat command, as it is used to display the file content in the same 
way that the cat command does. The only difference between both commands is that, in case of 
larger files, the more command displays screenful output at a time.
In more command, the following keys are used to scroll the page:
ENTER key: To scroll down page by line.
Space bar: To move to the next page.
b key: To move to the previous page.
/ key: To search the string.
Syntax:
1. more <file name>
Output:
16. less Command
The less
command is similar to the more command. It also includes some extra features such as 'adjustment 
in width and height of the terminal.' Comparatively, the more command cuts the output in the width 
of the terminal.
Syntax:
1. less <file name>
Output:
Linux User Commands
17. su Command
The su
command provides administrative access to another user. In other words, it allows access of the 
Linux shell to another user.
Syntax:
1. su <user name>
Output:
18. id Command
The id
command is used to display the user ID (UID) and group ID (GID).
Syntax:
1. id
Output:
19. useradd Command
The useradd
command is used to add or remove a user on a Linux server.
Syntax:
1. useradd username
Output:
20. passwd Command
The passwd
command is used to create and change the password for a user.
Syntax:
1. passwd <username>
Output:
21. groupadd Command
The groupadd
command is used to create a user group.
Syntax:
1. groupadd <group name>
Output:
Linux Filter Commands
22. cat Command
The cat
command is also used as a filter. To filter a file, it is used inside pipes.
Syntax:
1. cat <fileName> | cat or tac | cat or tac |. . . 
Output:
23. cut Command
The cut
command is used to select a specific column of a file. The '-d' option is used as a delimiter, and it can 
be a space (' '), a slash (/), a hyphen (-), or anything else. And, the '-f' option is used to specify a 
column number.
Syntax:
1. cut -d(delimiter) -f(columnNumber) <fileName>
Output:
24. grep Command
The grep
is the most powerful and used filter in a Linux system. The 'grep' stands for "global regular 
expression print." It is useful for searching the content from a file. Generally, it is used with the 
pipe.
Syntax:
1. command | grep <searchWord>
Output:
25. comm Command
The 'comm'
command is used to compare two files or streams. By default, it displays three columns, first displays 
non-matching items of the first file, second indicates the non-matching item of the second file, and 
the third column displays the matching items of both files.
Syntax:
1. comm <file1> <file2>
Output:
26. sed command
The sed
command is also known as stream editor. It is used to edit files using a regular expression. It does 
not permanently edit files; instead, the edited content remains only on display. It does not affect the 
actual file.
Syntax:
1. command | sed 's/<oldWord>/<newWord>/'
Output:
27. tee command
The tee
command is quite similar to the cat command. The only difference between both filters is that it puts 
standard input on standard output and also write them into a file.
Syntax:
1. cat <fileName> | tee <newFile> | cat or tac |.....
Output:
28. tr Command
The tr
command is used to translate the file content like from lower case to upper case.
Syntax:
1. command | tr <'old'> <'new'>
Output:
29. uniq Command
The uniq
command is used to form a sorted list in which every word will occur only once.
Syntax:
1. command <fileName> | uniq
Output:
30. wc Command
The wc
command is used to count the lines, words, and characters in a file.
Syntax:
1. wc <file name>
Output:
31. od Command
The od
command is used to display the content of a file in different s, such as hexadecimal, octal, and ASCII 
characters.
Syntax:
1. od -b <fileName> // Octal format
2. od -t x1 <fileName> // Hexa decimal format
3. od -c <fileName> // ASCII character format
Output:
32. sort Command
The sort
command is used to sort files in alphabetical order.
Syntax:
1. sort <file name>
Output:
33. gzip Command
The gzip
command is used to truncate the file size. It is a compressing tool. It replaces the original file by the 
compressed file having '.gz' extension.
Syntax:
1. gzip <file1> <file2> <file3>...
Output:
34. gunzip Command
The gunzip
command is used to decompress a file. It is a reverse operation of gzip command.
Syntax:
1. gunzip <file1> <file2> <file3>. .
Output:
Linux Utility Commands
35. find Command
The find
command is used to find a particular file within a directory. It also supports various options to find a 
file such as byname, by type, by date, and more.
The following symbols are used after the find command:
(.) : For current directory name
(/) : For root
Syntax:
1. find . -name "*.pdf"
Output:
36. locate Command
The locate
command is used to search a file by file name. It is quite similar to find command; the difference is 
that it is a background process. It searches the file in the database, whereas the find command 
searches in the file system. It is faster than the find command. To find the file with the locates 
command, keep your database updated.
Syntax:
1. locate <file name>
Output:
37. date Command
The date
command is used to display date, time, time zone, and more.
Syntax:
1. date
Output:
38. cal Command
The cal
command is used to display the current month's calendar with the current date highlighted.
Syntax:
1. cal<
Output:
39. sleep Command
The sleep
command is used to hold the terminal by the specified amount of time. By default, it takes time in 
seconds.
Syntax:
1. sleep <time>
Output:
40. time Command
The time
command is used to display the time to execute a command.
Syntax:
1. time
Output:
41. zcat Command
The zcat command is used to display the compressed files.
Syntax:
1. zcat <file name>
Output:
42. df Command
The df
command is used to display the disk space used in the file system. It displays the output as in the 
number of used blocks, available blocks, and the mounted directory.
Syntax:
1. df
Output:
43. mount Command
The mount
command is used to connect an external device file system to the system's file system.
Syntax:
1. mount -t type <device> <directory>
Output:
44. exit Command
Linux exit
command is used to exit from the current shell. It takes a parameter as a number and exits the shell 
with a return of status number.
Syntax:
1. exit
Output:
After pressing the ENTER key, it will exit the terminal.
45. clear Command
Linux clear command is used to clear the terminal screen.
Syntax:
1. clear
Output:
After pressing the ENTER key, it will clear the terminal screen.
Linux Networking Commands
46. ip Command
Linux ip
command is an updated version of the ipconfig command. It is used to assign an IP address, initialize 
an interface, disable an interface.
Syntax:
1. ip a or ip addr
Output:
47. ssh Command
Linux ssh
command is used to create a remote connection through the ssh protocol.
Syntax:
1. ssh user_name@host(IP/Domain_name)</p>
48. mail Command
The mail
command is used to send emails from the command line.
Syntax:
1. mail -s "Subject" <recipient address>
Output:
49. ping Command
The ping
command is used to check the connectivity between two nodes, that is whether the server is 
connected. It is a short form of "Packet Internet Groper."
Syntax:
1. ping <destination>
Output:
50. host Command
The host
command is used to display the IP address for a given domain name and vice versa. It performs the 
DNS lookups for the DNS Query.
Syntax:
1. host <domain name> or <ip address>
Output:
