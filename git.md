##Github安装
###Mac安装(Homebrew)
```
brew install git
```
##Github连接
###1、新建Github仓库
* 进入 Github 主页
* 点击 Repositories 选项
* 点击 New 按钮，进入新建仓库配置
* 输入仓库名称，添加描述
* 选择是否公开，选择是否初始化 README 文件
* 添加许可证
* 点击完成创建仓库

###2、配置Git
####在本地创建ssh-key
```
ssh-keygen -t rsa -C "your_email@your_email.com"
```
* 在主目录下执行这条命令
* `your_email@your_email.com` 为你自己的 Github 邮箱
* 我这里是一路回车，在 .ssh 目录下生成 id_rsa.pub ，里面的 key 就是我们需要的。
* 复制到 Github 设置 SSH and GPG keys 选项下，设置ssh-key

####本地测试验证
```
ssh -T git@github.com
```
* 第一次会提示是否继续，输入yes即可
* 如果显示 Hi 	XXXX! You've successfully authenticated, but GitHub does not provide shell access.
* 即是成功

####本地配置Git
```
git config --global user.name "your name"
git config --global user.email "your_email@your_email.com"
```
* `your name` 为自己的用户名
* `your_email@your_email.com` 为自己的邮箱

####添加远程仓库
```
git remote add origin git@github.com:your_name/your_repo.git
```
* `your_name` 为Github名字
* `your_repo` 为Github仓库

###3、工作流程
####添加修改文件到缓存区
```
git add <filename>
git add *
```
####提交修改文件，描述信息
```
git commit -m "xxx"
```
####推送修改文件到Github
```
git push origin master
git push
```
* 可以将 master 换其他分支，默认master
* 第一次输入 Github 帐号密码即可
















