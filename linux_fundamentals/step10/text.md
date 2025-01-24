### Command line browser
____________________________________________

Most of the time we need to browse urls to and fetch that content to command line. Sometimes we need partial information of the URL or the full information. curl command is available to browse the content over command line.

Syntax: curl <url>

```
curl www.google.com
```{{exec}}

Using curl command we can download the files.
```
curl https://archive.apache.org/dist/tomcat/tomcat-8/v8.0.0-RC1/bin/apache-tomcat-8.0.0-RC1-deployer.tar.gz -o apache-tomcat-8.0.0-RC1-deployer.tar.gz
```{{exec}}

Above command will download the file to the given filename. But without giving the filename also we can download it to the default file name.
```
curl -O https://archive.apache.org/dist/tomcat/tomcat-8/v8.0.0-RC1/bin/apache-tomcat-8.0.0-RC1-deployer.tar.gz
```{{exec}}