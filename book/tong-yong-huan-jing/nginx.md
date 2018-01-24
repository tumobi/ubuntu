+ sudo apt install nginx -y

+ 基本设置
+ 更改 nignx 的用户为 tumobi，防止出现各种权限问题
	`sudo vim /etc/nginx/nginx.conf`
	把第一行 user www-data; 更改为 user tumobi;
+  更改 var/www 目录所有都为 tumobi
  ```
  sudo chown -R tumobi.tumobi /var/www
  sudo chown -R tumobi.tumobi /var/log/nginx
  ```
+ 创建一个站点

+ 管理命令

