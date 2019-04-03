# learnVue
learn vue and about it more

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



ß