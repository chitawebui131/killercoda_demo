### List Files

In GUI OS you generally see the list of files when you open a particular folder. But in command line nd hence you may not see the files by default. Hence, you need to execute a command to check the **list** of files.

**Note! In Linux all is file !!**

Before listing, we create several files by different methods.

- touch <file_name> - create a empty file

```
touch file1.txt
```{{exec}}

- echo - echo will write the information to a file along with the redirect symbol **>**
```
echo "Some text" > file2.txt
```{{exec}}

##### Important Takeaways:

In Linux OS, there is no file-extensions. Extensions are given only for user understanding.

**ls** is a Linux shell command that lists directory contents of files and directories. Some practical examples of ls command are shown below.

Before list

```sh
Syntax: ls <Options> <Path>
```

Get list of files and directories but it may not show hidden files.
```
ls
```{{exec}}

Get list of hidden files and directories.

```
ls -A
```{{exec}}

Get list of hidden files and directories with top path.

```
ls -a
```{{exec}}

Get list of files with long format, usually shows properties of a file

```
ls -l
```{{exec}}

We can combine multiple options as well.

```
ls -Al 
```{{exec}}

```
ls -al
```{{exec}}

An analogue of this command is **ll** , but it is not available in all versions of Linux. In fact, the ll command is the same ls program, only configured and added to the ~/.bashrc file. T t she is an alias for ls -al.

```
ll
```{{exec}}

Usefull options:

-c, --time=ctime, --time=status

Sort the contents of a directory according to the time the state of the file changed (the `ctime' field in the inode). If the long format is specified with the -l option, then print the file's state change time instead of the file's modification time.
```
ls -c
```{{exec}}

-d, --directory

Display directory names as if they were regular files instead of displaying their contents.
```
ls -d
```{{exec}}

-f

Do not sort directory contents; output files in the order in which they are written to disk. This option also allows -a and -U and disables -l, --color, -s, and -t if they were given before -f.
```
ls -f
```{{exec}}

-h, --human-readable

Prefix each file size with a size letter, such as M for binary megabytes (`mebibyte'). (New in fileutils-4.0.)
```
ls -h
```{{exec}}

-i, --inode

Print the inode number (also called file serial number and inode number) of each file, to the left of its name. (This number uniquely identifies each file in each file system)
```
ls -i
```{{exec}}

-r, --reverse

Sort the contents of a directory in reverse order.
```
ls -r
```{{exec}}

