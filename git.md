##Github安装
###Mac安装(Homebrew)
```
brew install git
```
##Github连接
##配置Git
###在本地创建ssh-key
```
ssh-keygen -t rsa -C "your_email@your_email.com"
```
* 在主目录下执行这条命令
* "your_email@your_email.com" 为你自己的 Github 邮箱
* 我这里是一路回车，在 .ssh 目录下生成 id_rsa.pub ，里面的 key 就是我们需要的。
* 复制到 Github 设置 SSH and GPG keys 选项下，设置ssh-key

###本地测试验证
```
ssh -T git@github.com
```
* 第一次会提示是否继续，输入yes即可
* 如果显示 Hi 	XXXX! You've successfully authenticated, but GitHub does not provide shell access.
* 即是成功

###本地配置Git
```
git config --global user.name "your name"
git config --global user.email "your_email@your_email.com"
```
* "your name" 自己的用户名
* "your_email@your_email.com" 自己的邮箱

