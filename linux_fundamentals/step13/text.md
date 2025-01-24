### Compression/Decompression 
____________________________________________

#### Extracting the files from tar

Many times in Linux world all the softwares are packaged either in .zip or .tar format. To extract the files from .tar extension we can use tar command.

Syntax: tar -xf <filename>.tar.gz

```
tar -xf apache-tomcat-8.0.0-RC1-deployer.tar.gz
```{{exec}}

To extract archives we use -x option and -f means file.

Extracting the files from zip

Syntax: unzip <filename>.zip

```
curl -L -o shipping.zip https://github.com/roboshop-devops-project/shipping/archive/refs/heads/main.zip
```{{exec}}

```
unzip shipping.zip 
```{{exec}}

```
ls -Al
```{{exec}}
