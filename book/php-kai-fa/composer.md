# Composer

### 安装 composer
+ 下载安装脚本
 ```
 php -r "copy('https://install.phpcomposer.com/installer', 'composer-setup.php');"
 ```
 
+ 执行安装过程
 ```
 php composer-setup.php
 ```
 
+ 删除安装脚本
 ```
 php -r "unlink('composer-setup.php');"
 ```
 
+ 全局安装
```
sudo mv composer.phar /usr/local/bin/composer
```

+ 更新 composer 至最新版本
```
sudo composer selfupdate
```

### 设置 composer 中国镜像
修改 composer 的全局配置文件，在控制台下执行：
```
composer config -g repo.packagist composer https://packagist.phpcomposer.com
````
如果出现如下错误：
```
[ErrorException]                                                             
  touch(): Unable to create file /home/tumobi/.composer/config.json because P  
  ermission denied
```
解决方法：先给 .composer 目录设置权限 0777 
```
sudo chmod -R 0777 ~/.composer
```

### 参考链接
+ [Packagist 镜像使用方法](https://pkg.phpcomposer.com/)
