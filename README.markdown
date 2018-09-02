<h3>1.在github上先创建一个项目</h3>
<h3>2.在Ubuntu里创建一个目录 方便管理 mkdir xxx</h3>
<h3>3.编辑项目 也可以之后编辑</h3>
<h3>4.在终端切换到创建的目录</h3><p> cd xxx 然后 使用命令 git clone git@github.com:169000251/xxx.git[将远程服务器代码克隆到本地]这里去github上复制就可以</p><p>如果配置的是https，即https://github.com/169000251/xxx.git。这里我用ssh作为实例 </p>
<h3>5.如果在GitHub上创建项目时没有勾选（Initialize this repository with a README）则用命令来创建一个README.md</h3>
文件代码进入GitHub项目界面即可看到
#创建文件
<p>echo "# 项目名称" >> README.md </p>
#-初始化本地仓库
<p>git init</p> 
<p>git add README.md （添加到本地托管文件【暂存】）ps：git add .--添加所有</p>
<p>git commit -m "first commit"提交被托管文件到本地仓库<h5>（版本库）</h5>，引号里面可以写提交版本库的的说明--<h5>【最好对应提交的操作方便以后查看】</h5></p>
<p>git remote add origin https://github.com/169000251/项目名称.git（-添加到以origin命名远程仓库，可自己随意命名）</p>
<p>git push -u origin master（复制即可）<h5>【推送本地仓库内容到远程仓库】</h5></p>
<h3>如果勾选了（Initialize this repository with a README）</h3>
<p>则直接运行最后两行代码</p>
<p>git remote add origin https://github.com/169000251/项目名称.git（-添加到以origin命名远程仓库，可自己随意命名）</p>
<p>git push -u origin master（推送本地仓库内容到远程仓库）</p>
<h3>6.如果要添加文件<h3><p>则 用命令 touch xxx（文件名）创建 ，然后git add xxx（文件名）如果同时创建了多个则用【git add . 】来进行添加 </p>
<p>添加之后进行提交 git commit -m “提交操作的描述”</p>
<p>然后推送到远程master分支 git push origin master <h5>【origin是最开始命名的远程仓库，根据自己的命名进行更改】</h5></p>
