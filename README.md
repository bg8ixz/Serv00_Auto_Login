# Serv00 - 控制面板自动登录脚本
## 使用方法
　　在 GitHub 仓库中，进入右上角`Settings`，在侧边栏找到`Secrets and variables`，点击展开选择`Actions`，点击`New repository secret`，然后创建一个名为`ACCOUNTS_JSON`的`Secret`，将 JSON 格式的账号密码字符串作为它的值，如下格式：  
```
[  
  { "username": "qinshihuang", "password": "linux.do", "panelnum": "0" },  
  { "username": "zhaogao", "password": "daqinzhonggong", "panelnum": "2" },  
  { "username": "heiheihei", "password": "shaibopengke", "panelnum": "3" }  
]
```

## 参考来源
|  名称 |来源|地址|
| :------------: | :------------: | :------------: |
|Limkon|Github|https://github.com/Limkon|
