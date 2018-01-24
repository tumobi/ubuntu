###  Docker
* * * * *

+ 删除旧版本 Docker
	```
    sudo apt-get remove docker docker-engine docker.io
	```
    
+ 添加 Docker 软件源
	```
    sudo apt-get update
    sudo apt-get install apt-transport-https ca-certificates  curl software-properties-common
    curl -fsSL https://mirrors.ustc.edu.cn/docker-ce/linux/ubuntu/gpg | sudo apt-key add -
    sudo add-apt-repository "deb [arch=amd64] https://mirrors.ustc.edu.cn/docker-ce/linux/ubuntu $(lsb_release -cs) stable"
	```
    
+ 安装 Docker CE（社区版）
	```
	sudo apt-get update -y
	sudo apt-get install docker-ce -y
	```
    
+ 设置开机启动
    ```
    sudo systemctl enable docker
	sudo systemctl start docker
    ```
    
+ 把当前用户加入 docker 组
	```
    sudo groupadd docker
    sudo usermod -aG docker $USER
    ```
+ 测试 docker
	```
    docker run hello-world
    ```
### 使用 Docker 中国官方镜像加速
+ 编辑 vim /etc/docker/daemon.json 文件，添加以下内容：
   ```json
   {
      "registry-mirrors": [
        "https://registry.docker-cn.com"
      ]
    }
   ```
+ 重启服务
	```
	sudo systemctl daemon-reload
	sudo systemctl restart docker
    ```
###  Docker Compose
+ 安装 docker composer
	```
    sudo curl -L https://github.com/docker/compose/releases/download/1.18.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
	sudo chmod +x /usr/local/bin/docker-compose
    docker-compose --version
	```

+ 安装 docker composer 自动补全命令
    ```
    curl -L https://raw.githubusercontent.com/docker/compose/1.8.0/contrib/completion/bash/docker-compose > /etc/bash_completion.d/docker-compose
    ```

### 参考链接
+ 官方文档：https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#install-using-the-repository
+ Docker 问答录（100 问）：https://blog.lab99.org/post/docker-2016-07-14-faq.html
+ 中文文档：https://yeasy.gitbooks.io/docker_practice/content/install/ubuntu.html
+ Docker 中国官方镜像加速：https://www.docker-cn.com/registry-mirror