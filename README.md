# Hyper Upload Server

This is an super file upload server with asynchronous I/O architecture and coding by C++ language, it support over 4GB superlarge file upload  in Chromimu kernel browser and  less than 2GB in IE 11 browser or higher version. support break point renew, support Windows and Linux server platform, support arbitrary format of file upload, especially suitable for large video site applications. The single server supports 1000 concurrent uploading processes, supporting mainstream browsers on PC and smart phone.


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



# Hyper Upload Server 超级上传服务器

这是一款超级文件上传服务器，采用异步I/O架构，采用C++语言编码实现。它支持Chromium 内核浏览器4GB以上超大文件上传和断点续传，支持IE 11以上版本的浏览器中2GB的文件上传和断点续传，支持Windows和Linux服务器平台，支持任意格式的文件上传，尤其适合大的视频网站应用。单台服务器支持1000并发上传进程，支持PC端和智能手机端主流的浏览器。

## 主要特性
1. 服务器端采用异步I/O架设设计，具有高性能I/O处理能力，尤其适用于超大文件上传；
2. 服务器端采用高效内存分配技术确保在运行过程中服务器的内存开销最小化；
3. 完全采用标准协议实现，因此兼容几乎所有的PC端和移动端浏览器；
4. 服务器端采用C++语言自主实现，对上传文件的尺寸无限制，天生支持超大文件上传。
   而基于PHP、JAVA等技术实现的文件上传服务天生无法支持超大文件上传，无法逾越2GB的最大文件尺寸瓶颈；
5. 服务器端采用无缓冲即时写入方式，上传数据写入一步到位。不同于PHP、JAVA等技术实现方式需要两步写入；
6. 服务器端可跨平台编译运行，支持Windows和Linux平台；
7. 高性能，单台服务器支持1000个并发上传进程；
8. 支持Chromium内核浏览器中4GB以上超大文件上传，文件大小不受限制；
9. 支持IE 11版本及以上的浏览器最大2GB的文件上传；
9. 客户端支持采用HTTP标准协议上传；
10.支持断点续传，断网、关机重启均不受影响；
11.支持HTML5浏览器上传进度实时显示；
12.支持IE8及以上浏览器上传进度显示；
13.支持查看客户端在线连接， 查看方法： http://ip:port/lists
14.多浏览器兼容，包括Chrome，Firefox，Safari，IE，Opera,Edge；

## 安装

- 第一步：解压文件到一个硬盘目录，例如d:\UploadServer

- 第二步：修改配置文件 
		修改d:\UploadServer\conf\config.xml，文件里的目录设置，
		将所有 dir= 变量指向的目录修改为硬盘上的真实目录，如果没有就按配置文件创建； 
        
- 第三步：安装服务 <br/>
        执行cmd打开命令行窗口按步骤输入以下命令： <br/>
        d:  <br/>
        cd UploadServer <br/>
        HYFileServer.exe -i  <br/>   
        
- 第四步：启动服务 <br/>
        打开系统的服务管理器，找到Hyper Http Upload Service服务启动它。
                
- 第五步：在浏览器里输入 http://127.0.0.1:8080 查看服务器运行是否正常 <br>
        如果上传页面正常显示说明安装成功 <br>
        点击其中一个上传文件链接 按钮来上传一个文件。 <br>
        如果要在其它主机上访问上传服务器页面，请将127.0.0.1用安装服务器的IP地址取代。 <br>
        如果外部机器还不能访问，请检查防火墙的设置，看一下默认的8080端口是否开启。 <br>
        
- 第六步：如果要进一步了解上传服务器，请查看 d:\UploadServer\doc\文件上传服务器使用手册.pdf 文件 <br>

- Linux 下执行安装  <br>
./hyupdsrv  <br>
如果要作为守护进程，执行  <br>
./hyupdsrv -d <br>

## 技术文档
请查看 doc 目录下的说明手册。

## 联络
- QQ:1918098288
- Mail: 1918098288@qq.com








