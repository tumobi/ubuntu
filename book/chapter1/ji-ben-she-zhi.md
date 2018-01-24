### 源更改为中科大源
+ 请先备份原来然 sources.list 文件
```
sudo cp /etc/apt/sources.list /etc/apt/sources.list.bak
```
+ 使用 gedit 打开  /etc/apt/sources.list
```
sudo gedit /etc/apt/sources.list
```
+  把 /etc/apt/sources.list 的内容替换为以下内容，保存后关闭
  
```
deb https://mirrors.ustc.edu.cn/ubuntu/ xenial main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ xenial main restricted universe multiverse

deb https://mirrors.ustc.edu.cn/ubuntu/ xenial-security main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ xenial-security main restricted universe multiverse

deb https://mirrors.ustc.edu.cn/ubuntu/ xenial-updates main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ xenial-updates main restricted universe multiverse

deb https://mirrors.ustc.edu.cn/ubuntu/ xenial-backports main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ xenial-backports main restricted universe multiverse

## Not recommended
# deb https://mirrors.ustc.edu.cn/ubuntu/ xenial-proposed main restricted universe multiverse
# deb-src https://mirrors.ustc.edu.cn/ubuntu/ xenial-proposed main restricted universe multiverse
```
+ 更新索引以生效
```
sudo apt update -y
```

### 更新系统软件
```
apt upgrade -y
```

### 生成密钥

### IP、DNS、HOSTNAME

### 时间配置

### 卸载默认的软件
这步根据自己的需求进行操作


