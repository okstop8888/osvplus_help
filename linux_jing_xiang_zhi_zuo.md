#Linux上传流程

准备工作：

1. 本地正确安装Linux系统
2. 服务器安装并正确配置
3. Linux模板机，选择“网络启动”，将此计算机加入到服务器





#####上传Linux操作系统
1，更改模板机启动文件为：Linux-X86.bin (安装的Linux为32位，选择“linux-x86.bin”，如果为 X86_X64 请更换为“linux-x64.bin”启动文件)

![](/assets/l1.png)


2，使用控制台，新建一个镜像“ubuntu”

![](/assets/l4.png)

3，在ADMIM帐户下，新建一个启动菜单“Menu”

![](/assets/l5.png)


4，在Menu菜单下，新建一个简单包

![](/assets/l6.png)

5，将ubuntu镜像，拖至简单包下

![](/assets/l8.png)

6，开启“活动更新模式”

![](/assets/l7.png)

7，模板终端使用“网络引导”开机

![](/assets/l2.png)

8，输入管理员用户，密码进行系统上传
![](/assets/l9.png)

9，上传完成后，输入s，关闭终端

10，更改admin的访问模式为还原模式

![](/assets/l10-1.png)


制作完毕！



