# Node.js 环境安装

### 使用 nvm 安装 Node.js
+ 安装 nvm
	```
    wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
    source ~/.bashrc
    ```
    
+ 查看最新的稳定版本
	```
    nvm ls-remote
	```
+ 安装最新稳定版 Node.js
    ```
    nvm install v8.9.4
    ```
### 使用 淘宝 NPM 镜像
+ 安装 cnpm 
	```
    npm install -g cnpm --registry=https://registry.npm.taobao.org
    ```
    使用方法和 npm 基本一样，支持除了npm publish 之外的所有命令


### 参考链接：
+ https://github.com/creationix/nvm
