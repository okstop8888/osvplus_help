网络端口使用说明：

端口号 |  协议  |  用途
- | -  | -
服务端  |  -      |   - 
67    |    UDP      | PXE-DHCP 服务器
69    |    UDP      | PXE-TFTP 服务器  
5500  |    TCP      | 远程桌面
6969  |    TCP & UDP| BT服务器
7000  |    TCP & UDP | OSV 授权服务器（配置服务）
7001  |    TCP & UDP | OSV 数据服务器
7002  |    TCP & UDP | OSV 数据服务器
7006  |    TCP       | OSV 授权服务器（配置服务，用于服务器之间热备）
7010  |    TCP       | OSV 数据服务 
7012  |    TCP       | 远程维护 & BOOTLoader 启动




>如服务器在防火墙内或者需要跨互联网，请映射以上端口



