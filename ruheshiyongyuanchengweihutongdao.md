#如何使用远程维护通道


#使用场景

远程维护通道主要用于一些小型的远程维护，比如设置些注册表，激活软件等操作

[远程维护通道样例下载](http://vpn.os-v.com:82/%E8%BF%9C%E7%A8%8B%E7%BB%B4%E6%8A%A4%E6%A0%B7%E4%BE%8B%E4%B8%8B%E8%BD%BD/)



#使用方法


在服务端的  \boot\loader\Patch 目录下，有这些文件


![](/assets/uc1.png)


1， LearnMode ：此目录为终端为“学习模式”时，自动执行的脚本与文件

2， ReadMode  ：此目录为终端为“还原模式”时，自动执行的脚本与文件

3， WriteMode ：此目录为终端为“写入模式”时，自动执行的脚本与文件

4， MakeZip.bat ：此脚本为打包，配置完以上目录后，请执行此脚本进打行打包，打包成功后，客户端才可以正常执行维护通道


>注： 

>1, 远程维护通道仅在终端开机并进入桌面时，执行一次

>2, 在写入模式下，可能会造成重复执行，请在编写维护脚本时，进行判断

 
#编写方法

 1，进入服务端相关目录  \boot\loader\Patch\LearnMode
 
 2，将要执行的程序复制到此目录
 
 3，修改BAT文件
 
 4，运行MakeZip.bat进行打包
 
 5，操作控制台，使得终端进入学习模式，测试脚本运行情况
 
  
  
 #样例
 
 run.bat:
 
```
@echo off
rem 关闭回显
Driver_Setup.exe
rem 运行驱动安装工具
shutdown -r -t 40
rem 驱动安装完成后 超时40S 自动重启计算机
```

![](/assets/x8.png)


 
同时调用多个BAT

run.bat:



```
@echo off
call 1.abt
call 2.bat
exit
```



   
     
  


