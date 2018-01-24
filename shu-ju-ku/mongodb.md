# MongoDB

* * * * *

### 安装 MongoDB
+ 签名到APT
```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
```

+ 添加源
```
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.6 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.6.list
```

+ 开始安装
```
sudo apt update -y
sudo apt install -y mongodb-org -y
```

### 配置和使用
+ 配置
```
vim /etc/mongod.conf
```

+ 启动
```
sudo service mongod start
```

+ 停止
```
sudo service mongod stop
```

### MongoDB GUI
+ [Studio 3T](https://studio3t.com/)


### 参考链接
+ https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/
+ https://www.jianshu.com/p/5598f1dcbb98