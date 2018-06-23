# Manjaro_Inode

万恶的校园网，linux的虐杀者

解决不能用路由器创建wifi，只能用inode连接校园网的问题

fork from [Hitvz](https://github.com/Hitvz)/[iNodeClient](https://github.com/Hitvz/iNodeClient)

上面那个是基于apt包管理器的，也就是说deepin，ubuntu，mint等等都可以直接安装（不能保证）

我这个是移植到arch系中，可能有点瑕疵，但是能连接，我这里连接后用命令杀死可以不用挂inode后台(不能直接关闭窗口，得直接杀死后台)

刚开始需要安装两个依赖，已经写入脚本中，不用另行安装

```shell
sudo pacman -S libjpeg6-turbo
sudo pacman -S ncurses5-compat-libs
```

**使用办法**

```shell
git clone https://github.com/Hitvz/iNodeClient.git
sudo ./setup.sh

#可添加zsh的alias
# alias inode='sudo /etc/init.d/iNodeAuthService restart && /usr/iNodeClient/iNodeClient.sh'
#下次命令行输入 inode 直接启动
```

<img src="https://ws1.sinaimg.cn/large/0072Lfvtly1fsl0fh0h5bj30oi0fpwgt.jpg">

<img src="https://ws1.sinaimg.cn/large/0072Lfvtly1fsl0glytsnj30as0j4757.jpg">

<img src="https://ws1.sinaimg.cn/large/0072Lfvtly1fsl0hbbltrj30fk0dnjry.jpg">





