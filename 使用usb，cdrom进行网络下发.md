#一，准备USB设备
1.打开USB启动制作工具
![](/assets/26-1.png)
2.选择要写入的USB设置
![](/assets/26-2.png)


>Select Store Device : 选择要制作的USB设备


>Boot Server IP      ：输入服务器ＩＰ

>Boot Mode           :启动模式，默认选择Syslinux，如果引导失败，请选择 Grub4dos

>Clan And Write      :清空磁盘并写入，兼容性最好，选择此种模式会清空硬盘。清空后的磁盘，引导成功率最高

>Write Boot          :直接向磁盘写入引导，不会格式化磁盘，但成功率最低


3.向USB设备写入引导
![](/assets/26-3.png)


4.写入完成
![](/assets/26-4.png)


5.使用“Clean And Write”写入后的硬盘状态
![](/assets/26-5.png)

>写入成功后的磁盘，会形成二个分区，一个384MB的BOOT分区和一个DATA分区。DATA分区下会生成二个目录 “BOOT”和“VHD目录”。这二个目录的主要是通过USB设备直接写入桌面系统和菜单。

>BOOT目录：用于存储开机菜单，也就是服务器安装目录下的disk.zip文件

>VHD目录： 用于存储镜像文件


#二，使用USB设备启动启动
