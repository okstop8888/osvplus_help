#终端使用PXE启动时，无法进入BOOTLoader的处理方法
1. 在控制台-配置-DHCP设置中


![](/assets/111-1.png)

2. 在启动文件里，选择plus2.bin


![](/assets/111-2.png)

3. 在工具栏里，选择“重新启动重启服务”

![](/assets/111-3.png)

4. 重新启动终端，验证是否可以正常启动，如不行，请重复2，3步骤。并更换引导文件为 plus2.bin plus3.bin plus4.bin 几个文件进行轮换