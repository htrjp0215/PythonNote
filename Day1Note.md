#pymarkdown语法

##标题

1-6级标题

~~~markdown
#一级标题
##二级标题
###三级标题
####四级标题
#####五级标题
######六级标题
~~~



##序号

- 有序

  数字+TAB

- 无序

  "-"+TAB

  按 SHIFT+TAB返回上级

##代码块

"~~~"

###加粗

~~~    markdown
**文本内容**
~~~
###倾斜

~~~markdown
*文本内容*
~~~

###加粗+倾斜

~~~markdown
***文本内容***
~~~



###下划线（*）

~~~markdown
<u>下划线</u>
~~~

​	<u>下划线</u>

###图片

​	直接复制粘贴

###表格

​	上面菜单段落->表格->插入表格

​	快捷键为（command +alt+ T）

###删除线（※）

~~~markdown
~~文本内容~~
~~~

###链接

~~~
[显示文本](url)
~~~

###转换成pdf格式:

​	文件->导出->PDF







# 计算机基础

##计算机的组成

###cpu 

运算 逻辑

###memory 

临时存储，断电就没，速度快

 ### harddisk 

(固态/机械）永久存储，断电也在，速度慢

### operating system 

​	用于用户与计算机交互，软件都是基于操作系统开发的

​	目前主流操作系统主要为:

- windows
- linux
- mac
- ...

~~乱打比方不可取（~~

##编程语言

###编程语言是什么

​	与计算机沟通的形式语言

###编程语言的分类

* 编译型语言（compiled language）
  * 全写完一次性编译
  * 运行速度快
* 解释型（interpreted languages）
  * 边写边解释
  * 出了问题好修改，开发速度快

# Python简介

###Python的历史大事件

- <font color="red">Python2.4 2004 10.30 同年 Django诞生</font>
- <font color="red">2014年10月表示2.7会在2020停止支持</font>

### Python分类



- Cpython

  目前官方版本,使用C实现,使用最广泛,Cpython会将Python代码转换成字节码文件,在Python虚拟机上运行

- Jython

  JAVA实现的Python,将Python代码动态编译成JAVA字节码,在JVM上运行

- IronPython

  Python的C#实现,将Python代码编译成C#字节码,在CLR上运行

- PyPy

  Python实现的Python,很神奇,~~有一种无限递归的感觉,~~将Python的字节码再编译成机器码

# Python安装

### 获取安装文件

​	到[Python官网]([https://www.python.org](https://www.python.org/))下载

### 安装Python

- 在Windows上安装

  1. 安装

  略,下一步下一步就行了,中间注意修改安装路径,记录安装路径

  2. 配置环境变量

  在环境变量-系统变量中的Path中添加";",复制并在最后尾粘贴Python的安装路径

  3. 验证

  在命令提示符中输入Python,若成功进入Python命令行则安装成功,若进入成功可输入"exit()"敲击回车后退出.

  

- 在MacOS上安装

  - 下载dmg文件安装

  - 

    1. 到[Python官网]([https://www.python.org](https://www.python.org/))下载dmg文件并安装

    2. 修改环境变量

       MacOS系统自带Python2.7版本,输入Python默认启动2.7.若想改为默认启动Python3.x版本需要修改环境变量

       ​	step:

       1. 打开终端

       2. 执行

          ```shell
          open ~/.bash_profile
          ```

          

       3. 修改打开的文件添加环境变量,我自己没试过就不瞎写了,推荐使用下面的方法

       4. 执行,环境变量生效

          ```shell
          source ~/.bash_profile
          ```

    3. 验证

    在终端中执行```python```,显示刚刚更改的版本号即为成攻

  - 使用pyenv工具安装(个人推荐)

    - pyenv方便进行Python的多版本控制

    step:

    1. 安装homebrew

    2. 执行``brew install pyenv``安装pyenv工具

    3. 配置pyenv环境变量

       1. 修改文件

          1. 执行```open ~/.bash_profile```(没有的话先touch一个)

          2. 在文件中加入环境变量如下,保存

             ~~~
             export PYENV_ROOT=~/.pyenv
             export PATH=$PYENV_ROOT/shims:$PATH
             ~~~

       2. 执行``source ~/.bash_profile``环境变量生效

    4. 安装你想要的Python版本,例如Python 3.6.6

       - 执行命令``pyevn install 3.6,6``

    5. 执行``pyenv global 3.6.6``切换版本.

# 运行你的第一个Python程序

###Hello World

~~~
print("hello world")
~~~



- 脚本必带文件头（以上两行必须写在文件第12行）

~~~Python
#!/user/bin/env
#--coding:utf-8--
#以上是指定编码的文件头
print("Hello World")
print("你好 世界")

~~~





