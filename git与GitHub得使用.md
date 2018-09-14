# git与GitHub得使用

1.git上传管理工具

	1.看到git Bash 就证明安装成功了。

	2.两张操作方式：

		1.命令行窗口操作

			使用命令行操作

		2.可视化得窗口(具有UI界面)

2.gitHub代码托管仓库

3.git使用命令行操作步骤

	安装配置

		1.win+R打开命令行窗口

		2.配置基本用户信息

			git config --global  user.name "用户名"

​			git config --global  user.email "邮箱"

		3.查看配置

			git config  --list

		4.清除命令窗口：ctrl+L

	使用命令

		查看文件：ls

		进入文件目录：cd  Desktop/

		新建文件夹：mkdir  文件名

		初始化仓库：git init

		查看隐藏文件：ls -a

		

	git有两个环境：

		1.工作区  在工作区操作代码 然后提交

			创建工作文件：touch  文件名（test.txt）

			打开工作文件：open  文件（text.txt）

			编辑工作文件： vi 文件（text.txt） i进入编辑模式

			退出正在编辑得工作：esc

			保存： 点击：wq 保存并退出

		2.查看仓库状态并提交版本库

			在工作区声明要提交得文件命令：git add 文件（text.txt）

			提交（版本库）远程仓库：git commit  -m(表示添加描述)  

			修改：vi 文件（text.txt）

			查看仓库状态：git status（是否有文件修改）

			查看修改文件的详细内容状态：git  diff 文件（text.txt）

		3.版本回退（可以不同功能版本穿梭）

			回到之前版本（详细版本）：git  log

			每次提交都有对应的ID值

			HEAD停留的指针当前版本

			master的主分支

​			回到之前版本（精简版本）：git  reflog

			回退到指定版本：git reset  --hard  ID值

			回退到最近的一次版本：git reset  --hard  HEAD^

		4.修改

			打断返回是ctrl+c

			显示文本内容：cat

			丢弃工作区内容命令：git  checkout  --   文件（text.txt）

		5.删除文件

​			删除命令：rm  文件

​			删除.ssh命令：rmdir .ssh

## 	     6.远程仓库 

​		1.右键翻译成中文	

​		2.https://www.cnblogs.com/fnlingnzb-learner/p/5831284.htm

​		3.第一次推送远程仓库需要使用：git  push -u origin  master（第一次推送需要加-u)

​		4.推送远程仓库命令：git push origin  master(默认主分支）

























			

			

		

		

	