# learnVue
learn vue and about it more

环境安装
详见：https://github.com/creationix/nvm/blob/master/README.md

1.1 curl安装命令：curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash 
1.2 wget安装命令： wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
安装完成后关闭终端，重新打开终端输入 nvm 验证一下是否安装成功，当出现“Node Version Manager”时，说明已安装成功。

如果在新的终端输入 nvm 时提示：command not found: nvm，有可能是以下原因之一：

你的系统可能缺少一个 .bash_profile 文件，你可以创建一个此文件（可通过vi或vim命令），打开复制粘贴以下代码（安装nvm成功后终端的最好3行代码）进去，保存，然后再次运行安装命令；
---------
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
---------


nvm 常用命令

nvm install stable ## 安装最新稳定版 node，当前是node v9.5.0 (npm v5.6.0)
nvm install <version> ## 安装指定版本，可模糊安装，如：安装v4.4.0，既可nvm install v4.4.0，又可nvm install 4.4
nvm uninstall <version> ## 删除已安装的指定版本，语法与install类似
nvm use <version> ## 切换使用指定的版本node
nvm ls ## 列出所有安装的版本
nvm ls-remote ## 列出所有远程服务器的版本（官方node version list）
nvm current ## 显示当前的版本
nvm alias <name> <version> ## 给不同的版本号添加别名
nvm unalias <name> ## 删除已定义的别名
nvm reinstall-packages <version> ## 在当前版本 node 环境下，重新全局安装指定版本号的 npm 包



git use 

1 判断是否安装git： git

2.1 安装git： brew install git
2.2 直接下载xcode直接从AppStore安装Xcode，Xcode集成了Git，不过默认没有安装，你需要运行Xcode，选择菜单“Xcode”->“Preferences”，在弹出窗口中找到“Downloads”，选择“Command Line Tools”，点“Install”就可以完成安装了

3.1 创建ssh key、配置git
git config --global user.name "wenbo"
git config --global user.email "1050794513@qq.com"

file in which to save the key (/Users/WENBO/.ssh/id_rsa)

open .ssh/id_rsa.pub 或者 cat .ssh/id_rsa.pub

复制里面的key

3.2 登录GitHub（默认你已经注册了GitHub账号），添加ssh key，点击Settings


4 链接验证:ssh -T git@github.com 

5 文件下载
cd /Users/WENBO/Desktop/   
git clone git@github.com:wenmobo/LearnGit.git

6 文件上传
//文件添加到仓库（.代表提交所有文件）
git add .
//把文件提交到仓库
git commit -m "First Commit"
//上传到github
git push

