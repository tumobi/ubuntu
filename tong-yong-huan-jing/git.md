## Git 
+ 使用 apt 安装最新版 git
```
sudo add-apt-repository ppa:git-core/ppa
sudo apt update
sudo apt install git -y
```

+ 设置用户信息
```
git config --global user.name "tumobi"
git config --global user.email "tumobi@163.com"
```

+ 更改文本编辑器
```
git config --global core.editor vim
```

+ 查看配置信息
```
git config --list
```

### Git GUI 
+ [GitKraken](https://www.gitkraken.com/)

### Git托管服务
+ GitHub
大家都在用，开源项目首选。缺点是免费用户不支持私用仓库，国内的话网速可能会有影响。
配置 key 与 github

+ Gitee
如果觉得github网络慢或是需要免费私有仓库的话，可以试试国内的 Gitee，还有一个比较强大的功能就是可以同步 GitHub 项目

### 参考链接
+ https://git-scm.com/book/zh/v2
+ http://blog.csdn.net/yhl_leo/article/details/50760140
+ http://iissnan.com/progit/html/zh/ch1_5.html
+ https://www.howtoing.com/ubuntu-upgrade-the-latest-version-of-git
