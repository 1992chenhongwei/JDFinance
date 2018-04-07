# JDFinance
#技术语言： 
ES6、CSS3、Sass 
#框架：
vue@^2.5.9  vue-router@^3.0.1 
#构建工具：
webpack@^3.10.0 
#环境配置：
node@^8.9 
#系统：
windows安装Git，Gitbash操作命令行
#项目说明：
整个项目采用组件化开发，用简单的方法做出漂亮的项目；
1.在开发过程中整个项目采用的主要布局方式为flex（row&&column)；
2.通过对各个业务功能模块进行分析，抽离出公共组件，其中包括slider轮播图组件，header头部公共组件，footor底部组件，nav导航组件，
及panel等布局组件；
3.该项目使用vue框架进行开发，通过components注册组件的方式引入公共组件；
4.项目中各个页面的跳转是通过路由的方式实现;
5.项目使用Git进行代码管理，Gitbash操作命令行；
#Git命令行
第一步：建立git仓库

cd到你的本地项目根目录下，执行git命令，此命令会在当前目录下创建一个.git文件夹。

git init

第二步：将项目的所有文件添加到仓库中

git add .

这个命令会把当前路径下的所有文件，添加到待上传的文件列表中。

如果想添加某个特定的文件，只需把.换成特定的文件名即可

第三步：将add的文件commit到仓库

git commit -m "注释语句"

第四步：去github上创建自己的repository点击New repository，填好所有信息后点击create repository就会进入到类似下面的一个页面，拿到创建的仓库的https/ssh地址

第五步：将本地的仓库关联到github上

git remote add origin 自己的仓库url地址

第六步，上传代码到github远程仓库

git push -u origin master

执行完后，如果没有异常，等待执行完就上传成功了，中间可能会让你（用ssh地址不需要输入）输入Username和Password，
你只要输入github的账号和密码就行了.

第一次上传有可能会遇到push失败的情况，那是因为跟SVN一样，github上有一个README.md 文件没有下载下来 。我们得先
git pull --rebase origin master  ，然后执行git push -u origin master 就可以成功啦

现在，你已经决定要解决你的公司使用的问题追踪系统中的某个问题。 想要新建一个分支并同时切换到那个分支上，你可以运行一个带有 -b 参数的 git checkout 命令：

$ git checkout -b 分支名
Switched to a new branch "分支名"
它是下面两条命令的简写：

$ git branch newbranch
$ git checkout newbranch

打tag并提交远程版本库

git tag tagname
git push origin tagname
