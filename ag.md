Ag 

依据文件中的字符进行查找

## 1. 安装

````
apt-get install silversearcher-ag
````

\<2020-05-25 一 15:05>

## 2. 说明

通过文件中的关键字进行搜索 ( ag 类似 grep 和 find，但是执行效率比后两者高）。

## 3. 参数

```bash
-l                      # 只列出文件名 
-g <File Name>          # 文件名匹配 类似于 find . -name <File Name> 
-i PATTERN              # 忽略大小写搜索含PATTERN文本 
-A PATTERN              # 搜索含PATTERN文本，并显示匹配内容之后的n行文本，例如： -A 5 abc会显示搜索到的包含abc的行以及它之后5行的文本信息。 
-B PATTERN              # 搜索含PATTERN文本，并显示匹配内容之前的n行文本 
-C PATTERN              # 搜索含PATTERN文本，并同时显示匹配内容以及它前后各n行文本的内容。
--ignore-dir <Dir Name> # 忽略某些文件目录进行搜索。 
-w PATTERN： 全匹配搜索， # 只搜索与所搜内容完全匹配的文本。
--java PATTERN：        # 在java文件中搜索含PATTERN的文本。 
--xml PATTERN：         # 在XML文件中搜索含PATTERN的文本。
```



<2020-06-07 日 21:38>


2020年 08月 21日 星期五 18:58:42

