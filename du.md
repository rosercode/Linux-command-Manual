## du 命令

### 1. 简介

1.  作用:用于显示目录或文件的大小。或显示指定的目录或文件所占用的磁盘空间
2.  英文原意:disk usage

### 2. 参数:

1. 和显示格式相关的参数:

   ```bash
   -b 或-bytes            # 显示目录或文件大小时，以byte为单位 
   -h 或--human-readable  # 以k，M，G为单位，提高信息的可读性 
   -H 或--si 	          # 与-h参数相同，但是K，M，G是以1000为换算单位。 
   -m  或--megabytes      # 以1MB为单位
   --exclude=<目录或文件>  #  略过指定的目录或文件。
   ```

2. 其它参数

   ```bash
    -l 或--count-links  # 重复计算硬件连接的文件。
    -s 或--summarize    # 仅显示总计。# 好用的一个命令参数 注:参数为全部列出:
   ```

3. 帮助和版本: 

   ```bash
   --help 显示帮助。 
   --version 显示版本信息。
   ```

### 3. 使用

```bash
$ sudo du -s -h wangshuo	# 以K，M，G为单位,显示 wangshuo 目录的大小 60G
$ sudo du -s -h *home* 		# 显示所有用户所用的内存 108G
$ sudo du -s -h wang-shuo 	# 以K，M，G为单位,显示 wangshuo 目录的大小 38G
$ du -m -d 1 | sort -nr		# 显示指定目录下所有文件的大小,不向下进行递归
```

## 笔记

确定目录的总大小？

```shell
du -hs /path/to/directory
du -h | sort -h
du -h --max-depth=1 /path/to/directory
du -h --max-depth=1 /path/to/directory | sort -h

apt-get install ncdu
```

<2020-06-05 五 20:23>

\<2020-06-08 一 15:28>

## 参考

[qastack-how-do-i-determine-the-total-size-of-a-directory-folder-from-the-command-line](https://qastack.cn/ubuntu/1224/how-do-i-determine-the-total-size-of-a-directory-folder-from-the-command-line)

[菜鸟教程-du命令](https://www.runoob.com/linux/linux-comm-du.html)