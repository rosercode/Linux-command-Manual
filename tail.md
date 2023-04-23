## 1. 介绍

 tail **命令**可用于查看文件的内容

## 2. 参数

```bash
-n  #  指定显示文件的尾部函数
-c  #  指定显示文件尾部的字节数
-f  #  根据文件描述符追踪文件新增内容，文件改名或者删除时，则停止
-F 	#  根据文件名进行持续跟踪，文件改名或删除时，如果再次创建之前同名的文件名，则继续追踪
```

`-f` 和 `-F` 参数常用于查看某个时间段频繁变化的文件，比如日志文件

## 3. 应用





2021-10-14 22:06:50  -- 2021-10-14 22:06:56