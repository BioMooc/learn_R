# 第一章 简介、安装与运行




## 1.1 简介

- 本教程从R入门之后开始讲，认定的入门的标志是
    * 会安装R和Rstudio了
    * 遇到问题能首先尝试搜索解决了：
        * 阅读错误消息，不认识的单词查有道词典
        * 还看不懂则把错误消息放到搜索引擎中搜索



## 1.2 安装与运行方法


### 推荐的运行环境

R 越来越复杂了，直接使用windows版的R经常会遇到一些不好解决、甚至不能解决的问题。

> 理想的工作模式是，Linux服务器安装R和Rstudio，然后使用Windows等作为终端机登录服务器使用。

- 对于特别难安装的包，也可以使用容器化技术，比如 docker
    * [Docker containers for Bioconductor](https://www.bioconductor.org/help/docker/)


- 我的服务器的系统是 CentOS7.9 / Ubuntu 20.04，安装的R和Rstudio server最新版。
- 客户端机器是win10，使用chrome登录 Rstudio server编写R代码，使用 xshell 登录ssh进行命令行操作。



### 运行方式

主要是交互模式和脚本方式。

```
# 交互模式，就是打开R环境，一行一行运行
> a1=1
> a2=2
> a1 + a2
[1] 3


# 脚本运行方式，就是把R代码写到一个文件中，然后运行该文件
$ vim test1.R
a1=1
a2=2
a3 = a1+a2

print( sprintf("a1 + a2 = %d", a3) )

运行:
$ Rscript a0_1.R 
[1] "a1 + a2 = 3"
```







### windows 用户安装方法

依次下载并安装R和Rstudio，后者可选。

- 具体过程自己搜索吧(百度/必应/谷歌)。同时官方提供了几个问题与解答:
    * [Frequently Asked Questions on R](https://cran.r-project.org/doc/FAQ/R-FAQ.html)
    * [R for Windows FAQ](https://cran.r-project.org/bin/windows/base/rw-FAQ.html)
    * [R for macOS FAQ](https://cran.r-project.org/bin/macosx/RMacOSX-FAQ.html)






## 1.3 编辑器与IDE

- 推荐使用 Rstudio / Rstudio server。
- 主要权衡个人爱好与工作效率。
    * jupyter notebook 也可以通过插件支持R语言。
    * vs code 也有R语言的插件，不过图形不可拖动调长宽比，不画图还凑合能用。
    * 普通文本编辑器也能使用，像 vim, notepad, notepad++, sublime等。

