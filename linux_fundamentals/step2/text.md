### Hardware and Operating system Information
____________________________________________

When we purchase a new hardware like Laptops or Desktops we generally look into the configuration of the machine. So let us try to do the same for the PC with Linux. And it`s this is minimum knowledge required while you are working on any machine .

Login to the PC CLI and run the following commands.

To check the vendor of the operating system.

```
cat /etc/*release
```{{exec}}

To check the CPU information

```
cat /proc/cpuinfo
```{{exec}}

To check the memory information

```
cat /proc/meminfo
```{{exec}}

To check the disk information

```
lsblk
```{{exec}}

To check the architecture whether it is 32bit or 64bit

```
uname -i
```{{exec}}

32 bit ->  i386/i586/i686
64 bit ->  x86_64

With this information in hand you will have an idea of what you are dealing with and the specifications of that Linux machine.