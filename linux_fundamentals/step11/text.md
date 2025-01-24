### Pipes
____________________________________________

Pipes are used to send the output of one command to another command without storing the content anywhere physically on disk.

  Syntax :  com1 | com2

```
cat /etc/passwd | grep root
```{{exec}}

Note: All the commands will not accept inputs over pipes. In case if we need to take the input then we take the help of xargs command.

```
touch sample.txt
ls
```{{exec}}

```
echo sample.txt | rm -f
ls
```{{exec}}

Now you can use the xargs command.

```
echo sample.txt | xargs rm -f
ls
```{{exec}}