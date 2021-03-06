# ubuntu自动配置脚本

### 前言

写这个脚本**旨在减轻重装ubuntu系统后的配置压力**。在重装系统后可以运行这个脚本实现常用软件、主题、图标、字体、vim、zsh的配置，用户只需要在运行过程中输入确认信息即可。另，用户可以在程序中自动添加或删除需要的东西。

测试系统：ubuntu 16.04

### 结构

```
 .
├── install.sh # 运行脚本
├── log.txt # 输出日志
├── README.md
└── res # 资源文件
    ├── apps
    │   └── apps.txt # 需要安装的app，一行一个，必须是支持apt直接安装的
    ├── font
    │   └── Monaco # 两种字体
    │       ├── monaco_linux.ttf
    │       └── Monaco_Yahei.ttf
    ├── ppa # 添加ppa的脚本，可以到这里添加或者删除你的ppa
    │   └── ppa.sh
    ├── vim # 我的vm配置文件
    │   └── my_vimrc
    └── zsh # zsh主题和zsh配置
        ├── bullet-train.zsh-theme
        └── my_zshrc

7 directories, 10 files


```



### 运行

```shell
git clone git@github.com:dongchangzhang/ubuntu-config.git;
cd ubuntu-config;
chmod 755 install.sh
./install.sh -你需要的参数
```

### 运行级别
具体到代码中查询，这里列出的仅供参考
```
--help--
-0  install applications
-1  install monaco && micosoft yahei fonts
-2  config zsh
-3  config vim
-4  config icons
-5  install powerline fonts
-6  add ppa
-7  do all for your system, if your system is new one
-其他  help
-----
if you use zsh && vim, you should install powerline fonts at first
if you want to install apps, you should add ppa at first

```



### 软件

* tree       # 查看目录结构
* ranger #终端文件管理
* git        # 这个。。。
* htop    # 任务管理
* vim     # 不用说了
* tlp    # 电源管理
* zsh    # 强大的命令解释工具
* autojump # zsh下的一个插件
* tmux # 强大的终端多窗口等
* nethogs # 查看各个应用网速占用
* guake # 下拉终端
* gitg # 可视化查看git历史
* vlc # 视频播放器
* unity-tweak-tool # unity配置管理
* shutter # 截图
* indicator-keylock # 大小写指示器
* classicmenu-indicator # 经典应用选择指示器
* albert # 快速搜索工具
* typora # 好用的markdown工具
* calibre # 电子书阅读
* wiznote # 全平台笔记客户端
* catfish # 文件搜索
* python-pip # python2.7
* python3-pip # python3
* rar
* unrar
* mysql-server
* mysql-client

### 图标

* papirus-gtk-icon-theme #最好看的图标，可以搜索这个图标的github

### 字体

* Monaco_YaHei # 最好看的中英文字体

* Monaco # 适合编代码

### 其它

* ZSH

  使用oh-my-zsh配置，并且包含一份可以命令高亮的.zshrc

* VIM

  包含airline和其他常用的配置，使用vundle管理插件

* powerline fonts

  airline以及zsh主题需要
### 仍然需要下载安装的

* 网易云音乐
* WPS
* chrome
* VMware
* vscode
* MEGA
* 有道词典

### 仍需要配置

* ssh + git + github

### 下面的放到单分的opt目录中，不需要反复下载
* clion pycharm etc.
* tomcat
* struts2
* eclipse
* mysql-connecter
* android-studio



