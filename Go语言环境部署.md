# Go语言环境部署教程：
## 1.依赖包安装：
	sudo apt-get install bison ed gawk gcc libc6-dev make
	sudo apt-get install gcc-multilib g++-multilib
## 2.配置Go环境变量：
### 打开HOME目录下.bashrc文件：
	vim ~/.bashrc
### 在文件中添加内容：
	export GOROOT=$HOME/go
	export GOBIN=$GOROOT/bin
	export GOOS=linux
	export PATH=$GOROOT/bin:$PATH
	export GOPATH=（工程目录）
### 保存设置并运行命令使其生效：
	source ~/.bashrc
## 3.编译Go源代码：
### 注意：源代码部分文件没有权限，需要chmod 755添加权限
	cd $GOROOT/src
	./all.bash
### 当出现一下显示时，安装成功
	ALL TESTS PASSED

	---
	Installed Go for linux/386 in /home/wuxianglong/go.
	Installed commands in /home/wuxianglong/go/bin.
