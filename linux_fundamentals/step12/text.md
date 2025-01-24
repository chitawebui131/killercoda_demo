### Hard and Soft links
____________________________________________

Each file or directory has an “id” of their locker, this “id” is named inode and you can know the inode of your file/directory execute ls -i command

```
ls -i
```{{exec}}

Hard Links - Hardlinks create a value referenced the inode, let’s create our first hardlink

ln original-file-name added-file-name

```
touch linksample.txt
ls
```{{exec}}

```
ls -i
```{{exec}}

```
ln linksample.txt hard_linksample.txt
```{{exec}} 

```
ls -iAl
```{{exec}}

linksample.txt and hard_linksample.txt have the same inode number and hard_linksample.txt is a hard link to linksample.txt file.

Symbolic Links

ln -s original-file-name added-file-name
ln -s today weather

```
ln -s linksample.txt soft_linksample.txt
```{{exec}} 

```
ls -iAl
```{{exec}}

linksample.txt and hard_linksample.txt have the different inode number and soft_linksample.txt is a soft link to linksample.txt file. It can also be seen by the first letter in the file type/attributes - l