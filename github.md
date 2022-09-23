初始配置-关联github账号：  
Git Bash:  

	$ ssh-keygen -t rsa -C "youremail@example.com"

打开github账号设置，添加SSH Key，添加内容为.ssh/id_rsa.pub文件内容

***

建立本地库：  

	git init //创建
	git add file_name //暂存，待上传
	git commit -m "commit message"  //暂存内容更新至本地库，添加注解信息

本地库更新远程库：  

	git remote add origin [github库地址（***.git）]
	git push -u origin master //-u参数第一次加，后续不需要

远程库更新本地库（需要先设定origin）：  

	git pull origin master

克隆远程库：  

	git clone ***.git