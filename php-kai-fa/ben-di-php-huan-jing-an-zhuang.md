+ 安装 php7.2
  + sudo apt install -y software-properties-common -y
  + sudo add-apt-repository ppa:ondrej/php
  + sudo apt update -y
  + sudo apt install -y php7.2 php7.2-mysql php7.2-fpm php 7.2-curl php7.2-xml php7.2-json php7.2-gd php7.2-mbstring -y
  
+ 更改 fpm 运行用户为 tumobi
 ```
sudo vim  /etc/php/7.2/fpm/pool.d/www.conf
 ```
查找  user = www-data 和 group = www-data，并把 www-data 改为 tumobi

+ 更改 php 相关目录属主为 tumob
```
sudo chown -R tumobi.tumobi /run/php
```

+ 配置 nginx
  
### 参考链接
+ https://www.2cto.com/kf/201706/646319.html