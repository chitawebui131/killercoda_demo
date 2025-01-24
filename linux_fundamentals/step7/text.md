### List anf filter file content
____________________________________________
Usually the filters are based on

- Line Numbers
- Row Filters
- Column Filters


The **cat** command

The cat command is a utility command in Linux. One of its most common usages is to print the content of a file onto the standard output stream. Other than that, the cat command also allows us to write some texts into a file.

Syntax: cat <filename>

```
cat /etc/passwd
```{{exec}}

It shows the content of the file
```
cat -n /etc/passwd
```{{exec}}

____________________________________________

**Head** command
To filter the output based on line numbers and that to be from starting of the file then we use head command.

Syntax: head <filename>

By default head command gives you top 10 lines of the file but you can change it according to your needs.
```
head /etc/passwd
```{{exec}}
```
head -n 5 /etc/passwd
```{{exec}}

It gives the first 5 lines of the file

____________________________________________
Tail Command

Head command gives you the top lines of the file however if you want to print the last lines you can use tail command

Syntax: tail <filename>

tail command will print last 10 lines and however you can change them using -n option.
```
tail /etc/passwd
```{{exec}}
```
tail -n 5 /etc/passwd
```{{exec}}

It gives the last 5 lines of the file

____________________________________________
Grep command

The grep filter searches a file for a particular pattern of characters, and displays all lines that contain that pattern. The pattern that is searched in the file is referred to as the regular expression (grep stands for globally search for regular expression and print out).

Syntax: grep <word> <filename>
```
grep root /etc/passwd
```{{exec}}

It fetches all the lines which have the word root in them.

____________________________________________
Awk Command
In some cases the content needs to be filtered based on the columns in that case we use awk command.

Syntax: awk -F 'delimiter' '{print $column-number}' <filename>

```
awk -F : '{print $1}' /etc/passwd
```{{exec}}

It will print the first column of the file

```
awk -F : '{print $1,$2}' /etc/passwd
```{{exec}}

It will print the first and second column of the file

Additional things to learn.
Regular Expressions.

https://youtu.be/mpyCeSvGh-M
