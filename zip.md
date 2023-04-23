

## 1. 说明

- Linux zip 命令用于压缩文件。
- zip 是个使用广泛的压缩程序，压缩后的文件后缀名为 .zip。
- ( 注：默认是可以直接查看压缩文件中的内容，或者执行压缩文件中的可执行文件 )

## 2. 参数

```bash
-P 密码    # 设置 zip 文件的密码,后面向已经存在的zip文件中添加文件默认是没有密码的，-P 和密码之间是没有空格的
-j     # 只保存文件名称及其内容，而不存放任何目录名称。一般最好加上这个参数
-r     # 表示递归，压缩目录，向压缩文件中添加目录都要使用这个参数
-d     # 从压缩文件内删除指定的文件。
```

## 3. 使用

```shell
zip -r myfile.zip test/ 	# 将test目录下打包成myfile.zip
unzip  myfile.zip           # 将myfile.zip.解压到当前目录下
unzip -O GBK                # 指定解压文件的编码
unzip -O cp936 Python.zip
zip -d myfile.zip a.txt     # 删除压缩包内的文件
zip -m myfile.zip a.txt     # 向压缩包内添加文件
zip -m myfile.zip -j ../video/o_t2.jpg # 不包含路径信息压缩文件(默认是包含的)
unzip -v abc.zip            # 查看压缩文件目录信息，但是不解压该文件。 
```



2020-10-26 01:09:34