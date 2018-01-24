# MySQL

* * * * *

### 安装
+ sudo apt install mysql-server mysql-client -y
+ 安装过程中输入 root 的密码

### 初始化配置
+ 安全配置 sudo mysql_secure_installation
  + 输入 root 的密码
  +  Would you like to setup VALIDATE PASSWORD plugin? 直接回车表示不设置密码的强度插件（本地开发环境建议不设置）
  +  Change the password for root ? 直接回车表示不修改
  +  Remove anonymous users? 输入 y 回车，删除匿名账号
  +  Disallow root login remotely? 直接回车表示不禁用远程 root 登录
  +  Remove test database and access to it? 输入 y 回车，删除 test 数据库
  +  Reload privilege tables now? 输入 y 回车，重新加载权限表

### 新增账号、权限分配
添加一个普通账号并设置权限
grant all on *.* to 'tumobi' identified by '123456';

### MySQL GUI
+ MySQL Workbench
+ DataGrip

### mycli 命令行增强 
+ 加强版MySQL命令行客户端，支持自动完成以及语法高亮功能
+ Github：https://github.com/dbcli/mycli
+  安装
```
sudo apt install mycli -y
```

+ 基本使用
```
mycli --help
```

### 常见问题
+ 密码设置失败问题，检查密码强度是满足
  	如果不想使用复杂的密码，可以不安装或者卸载掉密码安全插件（比如开发环境）
	mysql> UNINSTALL PLUGIN validate_password; (卸载密码安全插件)


