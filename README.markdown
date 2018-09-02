<h3>1.在github上先创建一个项目</h3>
<h3>2.在Ubuntu里创建一个目录 方便管理 mkdir xxx</h3>
<h3>3.编辑项目 也可以之后编辑</h3>
<h3>4.在终端切换到创建的目录 cd xxx 然后 使用命令 git clone git@github.com:169000251/xxx.git[将远程服务器代码克隆到本地](这里去github上复制就可以，如果配置的是https，即https://github.com/169000251/xxx.git。这里我用ssh作为实例 )<h3>
5.如果在GitHub上创建项目时没有勾选（Initialize this repository with a README）则用命令来创建一个README.md
文件代码进入GitHub项目界面即可看到
echo "# 项目名称" >> README.md （创建文件）
git init （-初始化本地仓库）
git add README.md （添加到本地托管文件【暂存】）ps：git add .--添加所有
git commit -m "first commit"（提交被托管文件到本地仓库（版本库），引号里面可以写提交版本库的的说明--【最好对应提交的操作方便以后查看】）
git remote add origin https://github.com/169000251/项目名称.git（-添加到以origin命名远程仓库，可自己随意命名）
git push -u origin master（复制即可）【推送本地仓库内容到远程仓库】
如果勾选了（Initialize this repository with a README）
则直接运行最后两行代码
git remote add origin https://github.com/169000251/项目名称.git（-添加到以origin命名远程仓库，可自己随意命名）
git push -u origin master（推送本地仓库内容到远程仓库）
6.如果要添加文件则 用命令 touch xxx（文件名）创建 ，然后git add xxx（文件名）如果同时创建了多个则用【git add . 】来进行添加 
添加之后进行提交 git commit -m “提交操作的描述”
然后推送到远程master分支 git push origin master 【origin是最开始命名的远程仓库，根据自己的命名进行更改】
【点击右上角的按钮 ，即可按行查看】
