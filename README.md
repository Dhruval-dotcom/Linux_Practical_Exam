## 1) pwd

The pwd command is used to display the location of the current working directory.

```bash
$ pwd
```

## 2) mkdir

The mkdir command is used to create a new directory under any directory.

```bash
$ mkdir dir1 dir2 dir3
```


## 3) rmdir

The mkdir command is used to create a new directory under any directory.<br>
rmdir -p command will delete a directory including its sub-directories all at once

```bash
$ mkdir dir1 dir2 dir3
$ rmdir -p
```

## 3) rmdir

The mkdir command is used to create a new directory under any directory.<br>
rmdir -p command will delete a directory including its sub-directories all at once

```bash
$ mkdir dir1 dir2 dir3
$ rmdir -p
```
## 4) ls

The ls command is used to display a list of content of a directory.<br>
Common ls Options<br>
<b>-A</b>  Like the -a option above except it does not list . (current directory) and .. (parent directory).<br>
<b>-h</b>  n long format listings, display file sizes in human readable format rather than in bytes.<br>
<b>-l</b>  Display results in long format.<br>
<b>-r</b>  Display the results in reverse order. Normally, ls displays its results in ascending alphabetical order.<br>
<b>-S</b>  Sort results by file size.<br>
<b>-t</b>  Sort by modification time.<br>

```bash
$ ls dir1/
```
## 5) cd

The cd command is used to change the current directory.<br>
cd .. will bring the user above one directory.<br>
cd - will change the user to the old directory.<br>

```bash
$ cd dir
```
## 7) touch

The touch command is used to create empty files. We can create multiple empty files by executing it once.<br>
touch -t
with this command, you can change the access time of a file by determining a specified time to it.<br>
touch -t YYYYMMDDhhmm.ss  
```bash
$ touch file1 file2 file3
```
## 8) cat
The cat command is a multi-purpose utility in the Linux system. It can be used to create a file, display content of the file, copy the content of one file to another file, and more.<br>
<b>cat > fileName</b>	                            To create a file.<br>
<b>cat oldfile > newfile</b>	                      To copy content from older to new file.<br>
<b>cat file1 file2 and so on > new file name</b>	  To concatenate contents of multiple files into one.<br>
<b>cat -n/cat -b fileName</b>	                    To display line numbers.<br>
<b>cat -e fileName</b>	                            To display $ character at the end of each line.<br>
<b>cat fileName << EOF</b>	                        Used as page end marker.<br>
<b>cat >> (file name)</b>                          To append content in a file.<br>
<b>cat *.txt</b>                                   To show only the contents of a text file inside a directory<br>
<b>cat sample.txt test.txt</b>                     Show Multiple Files<br>

```bash
$ cat file
$ cat > file 
```
## 9) rm

This command is used to remove a file. The command line doesn't have a recycle bin or trash unlike other GUI's to recover the files. Hence, be very much careful while using this command. Once you have deleted a file, it is removed permanently.
<b>rm *extension</b>	    Used to delete files having same extension.<br>
<b>rm -r or R</b>	        To delete a directory recursively.<br>
<b>rm -i</b>	            Remove a file interactively.<br>
<b>rm -rf</b>            Remove a directory forcefully.<br>

```bash
$ rm <filename> 
$ rm *.txt
$ rm -r file
$ rm -i file
$ rm -rf file
``` 
## 10) cp

The cp command is used to copy directories and files.

<b>cp  existing file new file</b>  	    Used to delete files having same extension.<br>
<b>cp -r </b> Option 'r' with the copy command can be used to copy a directory including all its content from a source directory to the destination directory.<br>
<b>cp *. extension dir</b> <br>
Multiple files or directories can be copied to a destination directory at once. In this case, target must be a directory. To copy multiple files you can use wildcards (cp *.extension) having same pattern.<br>
<b>cp --backup filename dir</b> </b> If the file you want to copy already exists in the destination directory, you can backup your existing file with the use of this command.<br>
<b>cp -i filename dir</b>   cp '-i' option allows you to confirm once before overwriting your file.<br>
<b>cp -l file dir</b> If you want to create a hard link of a file instead of copying that file, you can use option 'l'.<br>
```bash
$ cp file1 file2
$ cp -r file1 file2
$ cp -i file1 file2
``` 
## 10) mv

Linux mv command is used to move existing file or directory from one location to another. It is also used to rename a file or directory. <br>
<b>mv -i</b>	Asks for permission to over write. <br>
<b>mv *</b>	Move multiple files to a specific directory.<br>
<b>mv --suffix</b>	Used to take backup before over writing.<br>
<b>mv -u</b>	Only move those files that doesn't exist.<br>
```bash
$ mv file1 dir
$ mv dir dir
$ mv -i file dir
``` 

## 11) rename 

The rename command is used to rename files. It is useful for renaming a large group of files.<br>

```bash
$ rename 's/old-name/new-name/' files  
For example, to convert all the text files into pdf files, execute the below command:
$ rename 's/\.txt$/\.pdf/' *.txt 
```

## 12) head 

The 'head' command displays the starting content of a file. By default, it displays starting 10 lines of any file.<br>
The 'head -n' option displays specified number of lines.<br>

```bash
$ head <file name>
$ head file1 file2
$ head -n <file name>  
```
## 13) tail 

The 'tail' command displays the last lines of a file. By default, it displays last 10 lines of any file.<br>
The 'tail -n' option displays specified number of lines.<br>

```bash
$ tail <file name>
$ tail file1 file2
$ tail -n <file name>  
```
## 14) tac  

The tac command is the reverse of cat command, as its name specified. It displays the file content in reverse order (from the last line).
```bash
$ tac file 
```

## 15) more 

The more command is quite similar to the cat command, as it is used to display the file content in the same way that the cat command does. The only difference between both commands is that, in case of larger files, the more command displays screenful output at a time.<br>
In more command, the following keys are used to scroll the page:<br>
ENTER key: To scroll down page by line.<br>
Space bar: To move to the next page.<br>
b key: To move to the previous page.<br>
/ key: To search the string.<br>
```bash
$ more <file name>  
```
## 16) less 

The less command is similar to the more command. It also includes some extra features such as 'adjustment in width and height of the terminal.' Comparatively, the more command cuts the output in the width of the terminal.
```bash
$ less file
```

## 17) su

The su command provides administrative access to another user. In other words, it allows access of the Linux shell to another user.
```bash
$ su user 
```

## 18) id 

The id command is used to display the user ID (UID) and group ID (GID).
```bash
$ id
```  

## 19) useradd 

The useradd command is used to add or remove a user on a Linux server.
```bash
$ useradd  username  
```
## 20) passwd 

The passwd command is used to create and change the password for a user.
```bash
$ passwd username
```
## 21) groupadd 

The groupadd command is used to create a user group.
```bash
$ groupadd group name
``` 

## 22) cut 

The cut command is used to select a specific column of a file. The '-d' option is used as a delimiter, and it can be a space (' '), a slash (/), a hyphen (-), or anything else. And, the '-f' option is used to specify a column number.
```bash
$ cut -d(delimiter) -f(columnNumber) fileName
```

## 23) grep 

The grep is the most powerful and used filter in a Linux system. The 'grep' stands for "global regular expression print." It is useful for searching the content from a file. Generally, it is used with the pipe.
```bash
$ cat file | grep <searchWord>  
```

## 24) comm 

The 'comm' command is used to compare two files or streams. By default, it displays three columns, first displays non-matching items of the first file, second indicates the non-matching item of the second file, and the third column displays the matching items of both files.
```bash
$ comm file1 file2  
```

## 25) sed 

The sed command is also known as stream editor. It is used to edit files using a regular expression. It does not permanently edit files; instead, the edited content remains only on display. It does not affect the actual file.<br>
eg echo class5 | sed 's/class/standard/'
```bash
$ command | sed 's/<oldWord>/<newWord>/'
```

## 26) tr 

The tr command is used to translate the file content Eg from lower case to upper case.
```bash
$ command | tr <'old'> <'new'>
```

## 27) uniq 

The uniq command is used to form a sorted list in which every word will occur only once.
```bash
$ command <fileName> | uniq 
``` 
## 28) wc 

The wc command is used to count the lines, words, and characters in a file.<br>
To display the complete count information of multiple files at once, specify the file names after space (' ').
The '-l' option number of lines in a file.
-w, --words:  print the word counts.
      
```bash
$ wc <file name> 
$ wc <file1> <file2>
$ wc - l <file name>  
```  

## 29) od 

The od command is used to display the content of a file in different s, such as hexadecimal, octal, and ASCII characters.
```bash
$ od -b <fileName>      // Octal format  
$ od -t x1 <fileName>   // Hexa decimal format  
$ od -c <fileName>     // ASCII character format 
```  

## 30) sort 

The sort command is used to sort files in alphabetical order.
```bash
$ sort <file name>
``` 

## 31) find  

The find command is used to find a particular file within a directory. It also supports various options to find a file such as byname, by type, by date, and more.
(.) : For current directory name <br>
(/) : For root<br>
```bash
$ find . -name "*.pdf"
```   
## 32) locate  

The locate command is used to search a file by file name. It is quite similar to find command; the difference is that it is a background process. It searches the file in the database, whereas the find command searches in the file system. It is faster than the find command. To find the file with the locates command, keep your database updated.
```bash
$ locate <file name> 
```

## 33) date  
The date command is used to display date, time, time zone, and more.
```bash
$ date
```
## 34) cal  
The cal command is used to display the current month's calendar with the current date highlighted.
```bash
$ cal< 
```   

## 35) sleep  

The sleep command is used to hold the terminal by the specified amount of time. By default, it takes time in seconds.
```bash
$ sleep <time>
```       

## 36) time  

The time command is used to display the time to execute a command.
```bash
$ time
```  

## 37) zcat  
The zcat command is used to display the compressed files.like zip gz etc.
```bash
$ zcat <file name>
```  

## 38) df 

The df command is used to display the disk space used in the file system. It displays the output as in the number of used blocks, available blocks, and the mounted directory.
```bash
$ df
```

## 39) exit Command
Linux exit command is used to exit from the current shell. It takes a parameter as a number and exits the shell with a return of status number.
```bash
$ exit
```
## 40) clear Command

Linux clear command is used to clear the terminal screen.
```bash
$ clear
```

## 41) ip Command

Linux ip command is an updated version of the ipconfig command. It is used to assign an IP address, initialize an interface, disable an interface.
```bash
$ ip a or ip addr
```   

## 42) host Command

The host command is used to display the IP address for a given domain name and vice versa. It performs the DNS lookups for the DNS Query.
```bash
$ host <domain name> or <ip address>  
```
