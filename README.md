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
$ rmdir dir1 dir2 dir3
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
## 14) ps 

ps for viewing information related with the processes on a system which stands as abbreviation for “Process Status”. 
```bash
$ ps  
```

## 15) pid
pidof command is used to find out the process IDs of a specific running program
```bash
$ pidof chrome
```
## 16) Kill
kill command in Linux (located in /bin/kill), is a built-in command which is used to terminate processes manually. kill command sends a signal to a process which terminates the process 
```bash
$ kill <process_isd>
```
## 17) chown
Chown command is used to change the file Owner or group. Whenever you want to change ownership you can use chown command. 
```bash
chown [OPTION]… [OWNER][:[GROUP]] FILE… 
chown [OPTION]… –reference=RFILE FILE… 
```

## 18)chgrp
chgrp command in Linux is used to change the group ownership of a file or directory. All files in Linux belong to an owner and a group. You can set the owner by using “chown” command, and the group by the “chgrp” command. 
```bash
chgrp [OPTION]… GROUP FILE… 
chgrp [OPTION]… –reference=RFILE FILE… 
```
