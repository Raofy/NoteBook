# 什么Docker
Docker是一款基于Go语言实现的、开源的应用容器引擎
# Docker有什么用
- 开发者可以将应用程序及其相关的依赖部署到这个可移植的应用容器中，然后发布到Linux服务器上面
- 能够自动化打包web应用程序
# Docker的特点
使用docker能够快速的交付代码，测试和部署代码
# Docker与虚拟机两者之间的区别
# Docker安装
## 1.CentOS上安装
### 1.1 yum安装，安装Engine-Community
#### 1.1.1 安装所需的软件包，yum-utils提供了yum-config-manager，device-mapper-persistent-data和lvm2
```shell script
yum install -y yum-utils device-mapper-persistent-data lvm2
```
### 1.2 设置yum仓库地址
```shell script
yum-config-manager --add-repo http://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo
```
### 1.3 安装社区版docker-engine
```shell script
yum install docker-ce docker-ce-cli containerd.io
```
## 2.测试一下docker是否已经安装成功
```shell script
docker -v
```
如果显示docker的版本号，那么安装就成功了

![安装成功](/image/Docker_Install.png)



# 常用的Docker命令
