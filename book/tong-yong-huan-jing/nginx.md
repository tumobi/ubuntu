# Nginx

### 安装 Nginx
    ```
    sudo apt install nginx -y
    ```
### 管理命令
+ 启动 
```
sudo systemctl start nginx
```
+ 停止 
```
sudo systemctl stop nginx
```
+ 查看状态 
```
sudo systemctl status nginx
```
+ 设置开机启动
```
sudo systemctl enable nginx
```

### 基本设置
+ 更改 nignx 的用户为 tumobi，防止出现各种权限问题
	`sudo vim /etc/nginx/nginx.conf`
	把第一行 user www-data; 更改为 user tumobi;
+  更改 var/www 目录所有都为 tumobi
  ```
  sudo chown -R tumobi.tumobi /var/www
  sudo chown -R tumobi.tumobi /var/log/nginx
  ```
+ 创建一个站点

### 参考链接
+ https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04
