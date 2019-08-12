部分操作问题：



sudo命令：不在 sudoers 文件中

```bash
ll /etc/sudoers

chmod 777 /etc/sudoers

vi /etc/sudoers

在root ALL=(ALL:ALL) ALL 下面添加一行	ls ALL=(ALL)ALL	然后保存退出。第一个ALL是指网络中的主机，我们后面把它改成了主机名，它指明ls可以在此主机上执行后面的命令。第二个括号里的ALL是指目标用户，也就是以谁的身份去执行命令。最后一个ALL指命令名。

chmod 440 /etc/sudoers
```

