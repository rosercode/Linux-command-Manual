## 1. 引言

用于显示当前进程 (process) 的状态。 (对应的英文:Process Status)


## 2. 参数

```bash
-A # 列出所有的行程 
-f # 以长格式的形式列出。 
-w # 显示加宽可以显示较多的资讯
-l # 长格式 
-u username # 显示指定用户的进程 
-C 进程名 显示指定进程的信息 
-au 显示较详细的资讯 
-aux 显示所有包含其他使用者的行程 
-L PID 显示指定PID下的线程 
-e 关键字 显示所有进程信息 (和 ps 命令一同使用的关键字 args, cmd, comm, command, fname, ucmd, ucomm, lstart, bsdstart 和 start。)
-o 参数控制输出
```

### 3. 应用

```bash
$ ps -u user # 显示 user 用户的进程 
$ ps -aux --sort -pcpu | less # 根据 CPU 使用来升序排序 
$ ps -aux --sort -pmem | less # 根据 内存使用 来升序排序 
$ ps -aux --sort -pcpu,+pmem | head -n 10 # 只显示前十个进程 
$ ps -L 1213 # 找出特定进程的线程，可以使用-L 参数，后面加上特定的PID。 
$ ps -axjf # 树形结构显示进程 (作用相同的一个命令: 
$ pstree 
$ ps -eo pid,user,args # 登陆服务器的人数 
$ ps -eo pid,user,args >> 1.txt # 登陆服务器的人数 (配合重定向来使用)
```



 \<2020-06-02 二 22:17\>



(https://zhuanlan.zhihu.com/p/93473461
