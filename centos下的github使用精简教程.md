
###  [1:环境搭建(略-具体看网页)](https://blog.csdn.net/weiwenhp/article/details/52966540) 
###  **2:git操作**  
##### 1. 克隆项目到本地       如果只是把github上的源码拷下来看看，没准备提交代码到github，那不需要那么麻烦去设置。装好apt-get install git就行了，不需求配置ssh key。     克隆项目是执行下面命令 
`git clone https://github.com/weiwenhp/arwenPyTest.git`     项目链接是在哪呢？你随便搜索出来一个项目，点击右边的clone or download的按钮就可以看到 
##### 2. 添加文件并同步到github上 
###### 注意我通过ftp上传文件后同步，失败，发现git仓库clone下来的文件夹权限不够。      chmod 777 文件夹名
假如在clone下来的目录下新建一个文件newfile.py，将它添加到仓库 
`git add newfile.py` 
`git commit -m "add new file test"  `#提交到本地代码库，-m后面是注释 
`git push origin master ` #将代码推送到远程代码库，也就是github上，origin master是指的主干代码，这步会提示输入用户名密码，就是登陆github的用户密码 
