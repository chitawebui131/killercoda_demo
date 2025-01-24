### Directory and change directory


Alike any operating system Linux also has its own directory structure.

In windows, we use \ (backslash) to give the path of a file or a directory but in Unix & Linux we use **/** (forward slash).

In Linux, we have a **ROOT DIRECTORY** where the path of any directory start here. A simple forward slash **(/)** is called as a ROOT DIRECTORY.

Additionally, to the list of directories provided in the above diagram we have more directories. Each and every default directory under / have some purpose in the operating system.

Unlike Windows, Linux is Command line based OS, So if you want to move from one directory to another directory we would be using commands to get it done.

To check where you are currently in the system we use **pwd** command.
```
pwd
```{{exec}}

#### Create Directories

You can create a directory using mkdir command.

```
mkdir softserve dir3 
```{{exec}}

This will create a new directory with the name **softserve**. You can check using ls command.
```
ls
```{{exec}}

Now you can see demo directory listed.

#### Navigate to Directories

To change the working directory from one location to another we use cd command

Syntax: cd <directory>

```
cd softserve
```{{exec}}

you will switch to **softserve** directory
```
pwd
```{{exec}}

you can check your current working directory using pwd command

```
cd
```{{exec}}

simple cd command will take you to the home directory of the user

```
pwd
```{{exec}}

```
cd ~
```{{exec}}

cd ~ command will take you to the home directory of the user

```
cd /
```{{exec}}

cd /  command will take you to the root directory of the computer

```
cd ~
```{{exec}}