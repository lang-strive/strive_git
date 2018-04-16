## git客户端:
#####       https://www.sourcetreeapp.com/                   //sourcetree


## git——代码版本管理工具
> 分布式管理
> 速度快

## git:
``` bash
0. 图形操作
	https://www.sourcetreeapp.com/
1. 命令 √
	安装git客户端:
	https://git-for-windows.github.io/

	验证是否安装ok?
	在任意地方 -> 右键 -> git bash
```

## git bash （命令-linux）
``` bash
mkdir	创建目录
rmdir	删除目录
touch	创建文件
rm		删文件
ls		列出当前目录下所有内容
ll  		查看当前目录的子文件
pwd   	查看当前目录
clear	清屏
cd		切换目录
cd ..		退回上级
rm -rf   删除非空目录
vi  a.txt	->	"i" -> 编辑 -> esc -> :wq
cat a.txt	查看文件内容
```

## 仓库(文件夹)

> 普通目录变成git仓库:	
``` bash
git init
```
> 查看此时git仓库状态
``` bash
git status
```

> 查看提交日志
``` bash
git log	
```

> 版本回滚
``` bash
git reset --hard commit_id 	
```


## 分支:
> 查看分支:
``` bash
git branch
```

> 创建分支有两种方法:
``` bash
1.创建
	git branch 分支名称
	
2.切换分支:
	git checkout 分支名称
	
3.创建并且切换:  √
	git checkout  -b 分支名称
```

> 合并分支(把当前工作成功提交到master上):
``` bash
git merge  分支名称
```

> 查看当前分支:
``` bash
git branch
```
> 删除分支:
``` bash
git branch -d 分支名
```


-----------------------------------------------
github(码云，gitlab):
	注册

如何让本地和github服务器关联?
	0. 配置本地
		查看本地git配置: 
		git config -l   查看配置
		git config --global user.email “aaa@aa.com”
		git config --global user.name “ccc”
	1. 本地生成一个秘钥(SSH key)
		ssh-keygen -t rsa -C “xxx@xxx.com”  一路回车
	2. 拿到秘钥
		当前C盘，当前用户列表里面找到.ssh文件夹，里面有两个文件：
id_rsa和id_rsa.pub
		id_rsa.pub	√	用普通记事本打开
	3. 把秘钥填写到相应网站上(github)
		点击头像 -> settings -> SSH and GPG key -> 添加
---------------------------------------------------
往github上放东西(远程操作):
1. 确保github上已经建了一个项目:
2. git clone 项目地址
3. 本地正常操作
	git add .
	git commit -m "xxxx"
4. 提交
	git push
5. 更新
	git pull
---------------------------------------------------
gitPage: （个人网站）
1. 在github上创建一个仓库
	仓库名称:  你的名称.github.com
2. 点击仓库里面 setttings
---------------------------------------------------
现在需要做的:
一、
1. 	git config --global user.email "xxxx"
	git config --global user.name ""
2. github创建一个仓库
	复制仓库地址

	a).git clone 复制地址

	b).新增一个文件
	c). git add 文件名    //  git add .
	d). git commit -m '此次提交描述信息'
	e). git push
		-> username:邮箱
		-> 密码


