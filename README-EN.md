# Hyper Upload Server

This is an super file upload server with asynchronous I/O architecture and coding by C++ language, it support over 4GB superlarge file upload and break point renew, support Windows and Linux server platform, support arbitrary format of file upload, especially suitable for large video site applications. The single server supports 1000 concurrent uploading processes, supporting mainstream browsers on PC and smart phone.


## Features
1.The Hyper Upload Server is designed by asynchronous I/O and has high performance I/O processing capability, especially for super file uploading. <br>
2.The Hyper Upload Server adopts efficient memory allocation technology to minimize the memory cost during operation. <br>
3.Fully implemented by standard protocol, so it is compatible with almost all PC and mobile browser. <br>
4.The Hyper Upload Server is written by C++ language. It has no limitation on the size of uploaded files and is born to support super file uploading. While other file upload server based on PHP and JAVA technology is incapable of supporting large file uploads, and can not exceed the bottleneck of 2GB's largest file size. <br>
5.The Hyper Upload Server uses no buffering and instant write mode, upload data and write to the disk is only one step. Different from PHP, JAVA and other technology that needs two steps to write. <br>
6.The Hyper Upload Server can be compiled and run across platforms, supporting Windows and Linux platforms. <br>
7.High performance, single server supports 1000 concurrent upload processes. <br>
8.File size is not restricted, support for over 4GB file upload. <br>
9.The client support HTTP standard protocol. <br>
10.Support breakpoint renewal, the upload progress isn't affecter by broken network or browser restart. <br>
11.Support upload progress display in real time on HTML5 browsers. <br>
12.Support upload progress display in IE8 or above browser. <br>
13.Support view client online connection, Method: http://ip:port/lists <br>
14.Compatible with multiple mainstream browsers, including Chrome, Firefox, Safari, IE, Opera, Edge. <br>

## Installation

- The first step:
Decompress files to a hard disk directory, such as d:\UploadServer.
- The second step:
Modify the configuration file 'd:\UploadServer\conf\config.xml', <br>
Change all the directories that dir= variables are directed to the real directory on the hard disk. If not, create them by configuration file.
- The third step:
Install the service <br>
In windows,you can Open the command prompt through the CMD command,then execute the following commands: <br>
d:  <br>
cd UploadServer <br>
HYFileServer.exe -i <br>

In Linux,you can execute the following commands <br>
./hyupdsrv  <br>

If you want to use it as a daemon, please execute: <br>
./hyupdsrv -d <br>

- The fourth step: Start the service.
In windows you can find 'Hyper Http Upload Service' then start it. <br>
In linux you can  execute the following command. <br>
./hyupdsrv  <br>

- The fifth step: 
Enter http://127.0.0.1:8080 in browser to see if the server running correctly. <br>
If the upload page is normal, the installation is successful.then you can upload your file with it. <br>
If you want to access the upload server on other hosts, please replace 127.0.0.1 with the IP address of the server in browsers. <br>
If the external machine can't access the server, please check the settings of the firewall to see if the default 8080 port is opened. <br>

- The sixth step:
To further understand the uploading server, please check the d:\UploadServer\doc\ to read the upload server's manual file.

## Technical Documnet
Please check the manual in the ./doc catalog.

## Contact
- QQ:1918098288
- Mail: 1918098288@qq.com







