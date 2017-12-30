## vagrant 配置

### 一、虚拟机还是得依靠 VirtualBox 来搭建，免费小巧。 

下载地址：https://www.virtualbox.org/wiki/Downloads


### 二、下载地址：https://www.vagrantup.com/downloads.html 根据提示一步步安装。

装好以后运行 

```
$ vagrant init
$ vagrant box add hashicorp/precise64
// vagrant init hashicorp/precise64
$ vagrant up
$ vagrant ssh
vagrant@precise64:~$ cd /vagrant
vagrant@precise64:/vagrant$ sudo apt-get update 
vagrant@precise64:/vagrantsudo apt-get install nodejs
```

下面的方法适用于最新版本的Ubuntu、Ubuntu 12.04 LTS、Ubuntu 12.10、Ubuntu 13.04等版本。它可以帮助开发者在Ubuntu上安装Node.js，无需从头编译安装。你可以在云主机上执行以下的命令：

1. sudo apt-get update

2. sudo apt-get install -y python-software-properties software-properties-common  

3. sudo  add-apt-repository ppa:chris-lea/node.js  

4. sudo apt-get update  

5. sudo apt-get install nodejs  
 
### 输入下面命令安装node.js

`sudo apt-get install nodejs-legacy`

安装完输入 node -v 可查看版本号
