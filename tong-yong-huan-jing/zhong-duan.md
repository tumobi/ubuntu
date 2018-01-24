# 终端

* * * * *

### 使用 zsh
+ 安装 zsh 
```
sudo apt install zsh -y
zsh --version
```

+ 设置 zsh 为默认 shell
```
chsh -s $(which zsh)
```

+ 重启系统或是注销并重新登录

+ 验证更改结果
 ```
 echo $SHELL
 ```
 有类似输出 `/usr/bin/zsh` 则表示修改生效

### 使用 oh-my-zsh
+ 安装 oh-my-zsh 
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
安装过程可能会比较长，耐心等待。安装完成后，即可看到终端明显的改变。
+ 更改主题
```
vim ~/.zshrc
```
找到 `ZSH_THEME="robbyrussell"` 更改为 `ZSH_THEME="ys"`，关闭终端并重启

+ 安装插件
	+ zsh-autosuggestions 
		```
        git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
		vim ~/.zshrc
        ```
        找到 `plugins=(` 在 `git` 下加入一行 `zsh-autosuggestions`，重启终端生效

### 参考文档
+ https://www.jianshu.com/p/0d4334cdeeeb
+ https://github.com/robbyrussell/oh-my-zsh
