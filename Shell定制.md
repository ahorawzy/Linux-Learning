# Shell定制

## 修改环境变量

printenv 命令查看环境变量

用户可以向PATH变量中添加和删除路径

$ PATH=$PAHT:/usr/loval/bin/myproc

PATH用冒号分分隔
经过修改的环境变量只在当前的Shell中有效。

## 设置别名
$ alias ll='ls -l'

## 个性化设置：修改.bashrc文件
Shell为每个用户维护了一个配置文件，这个文件叫做.bashrc，位于用户主目录中。只要把命令添加到该文件中，就可以把色织保留下来，并且在该用户登录的任何地方都有效。

要让修改立即生效，可以使用source命令执行这个脚本
$ source .banshrc

系统还提供了/etc/bash.bashrc文件，从全局上定制Shell，但最好不要修改此文件应该吧环境变量和别名保存在/etc/bash.bashrc.local中 
