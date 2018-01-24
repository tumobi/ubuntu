### 安装
+ apt 方式安装
```
sudo apt install redis-server -y
```
apt 方式安装的版本会比较旧，如需要安装最新版 redis 请参考：https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-redis-on-ubuntu-16-04

### 配置和启动
+ 更改配置
```
sudo vim /etc/redis/redis.conf
```

+ 启动
```
sudo systemctl start redis
```
+ 开机启动
```
sudo systemctl enable redis
```

+ 关闭
```
sudo systemctl stop redis
```

### Redis GUI
+ [FastoRedis](https://fastoredis.com/) 
+ [RedisDesktopManager](https://redisdesktop.com/)

