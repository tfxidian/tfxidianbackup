---
title: 2018-4-4-Windows 开机自动运行批处理
tags: 学习,tips
date: 2018-4-4
grammar_cjkRuby: true
---
最近看学长写的开机自动启动的程序，想看看是怎么自动运行的。结果如下：
直接将脚本放到启动文件夹里面

「开始」菜单/程序/启动/脚本.bat
  这里的脚本.bat也可以是其他类型的脚本程序，比如Python程序。
  
  那么在ubuntu下呢？
  
  可以执行

``` nginx
  gedit ~/.profile
```


  在该文件最后添加需要执行的任务。
  比如，我们执行了

``` sml
  gnome-terminal -x bash -c 'echo "123" -S  python /usr/server.py'
```

用于开机自动登录，并执行==server.py==脚本文件。
