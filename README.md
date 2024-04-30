# Serv00 - 免费主机自动续期
## 说明
　　本项目基于[LINUX DO](https://linux.do)论坛佬友`maohai`的[脚本](https://linux.do/t/topic/66483/15)进行修改，在其基础上增加了`发送通知`、以及`运行日志`功能。

## 发送说明
|  主机状态/设置条件 |  说明 |发送内容 |执行动作 |
| :------------: | :------------: | :------------: | :------------: |
|  200 |  正常 |不发送|无|
|   502|  机子凉了 |服务不可用|通过SSH执行PM2命令|
|   [Errno 1] Address family for hostname not supported| 解析凉了  |解析失败|无|
|  自定义日期 |  固定日启动连接 |每月固定SSH连接提醒|连接SSH|

## 使用方法
　　将脚本放到`domains`目录下，使用`chmod +x Auto_connect_SSH.py`给`Auto_connect_SSH.py`添加可执行权限。  
  
　　在Serv00控制台的定时任务里面新建一个定时任务，`命令`如下：
```shell
/home/你的用户名/domains/Auto_connect_SSH.py
```
#### 参考设置图
![参考图片](https://cdn.linux.do/uploads/default/optimized/3X/f/6/f6516994395858a19637f5acf5baeecec96ea3fa_2_690x445.png)
## 参考来源
|  名称 |来源|地址|
| :------------: | :------------: | :------------: |
|Saika|Github|https://github.com/k0baya|
|Eric Lee|Github|https://github.com/giturass|
|maohai|LINUX DO|https://linux.do/t/topic/66483/15|
