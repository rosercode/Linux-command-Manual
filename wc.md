wc

## 1. 引言

用于统计字数

利用wc指令我们可以计算文件的Byte数、字数、或是列数，若不指定文件名称、或是所给予的文件名为\"-\"，则wc指令会从标准输入设备读取数据。
注:看linux命令先看应用,在看解释。 注:文件和目录是不同的。

## 2. 语法

>  wc \[-clw\]\[--help\]\[--version\]\[文件...\]

## 3. 参数

```bash
-c 或 --bytes或--chars 只显示Bytes数。 
-l 或 --lines 只显示行数。注:wc统计的行算是用换行符来确定的。就是说最后一行要有换行符 最常使用的一个参数
-w 或 --words 只显示字数。 
-L 或 --max-line-length 显示一个文件中的最长行的长度 
--help 在线帮助。
--version 显示版本信息。
```

#### 4. 应用

```bash
wc testfile # testfile文件的统计信息 3 92 598 testfile
# 解释:testfile文件的行数为3、单词数92、字节数598
wc testfile testfile1 testfile2 # 统计三个文件的信息
wc -l 1.org # 显示 1.org 这个文件的行号 通常和其它命令配合使用,作为管道的最后一个命令。
```