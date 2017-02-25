#####一、创建版本库
```
用户标识
git config --global user.name lr
git config --global user.email i@lr.cool
git config --global push.default matching

创建版本库
git init

创建测试文件lr.txt
echo 'hello world'> lr.txt

添加进暂存区
git add lr.txt

提交到仓库
git commit -m "lr提交"

查看状态
git status

查看文件修改内容
git diff lr.txt
```
#####二、版本回退
```
查看历史记录
git log
git log --pretty=oneline

回退到上一个版本
git reset --hard HEAD^

回退到上上个版本
git reset --hard HEAD^^

回退到上100个版本
git reset --hard HEAD~100

查看版本号
git reflog
git reflog lr.txt

通过版本号回退
git reset --hard 版本号

```
#####三、工作区与暂存区
```
工作区是看到的目录，工作区下的.git不属于工作区，是版本库。
git add实际上是把文件添加到暂存区
git commit实际上是把暂存区的所有内容提交到当前分支上
```
#####四、撤销修改和删除文件
```
撤销修改(工作区)
git checkout -- lr.txt
但如果把文件提交到暂存区就撤销不了的

删除文件
直接删除
rm lr.txt
然后commit
未commit前可用git checkout恢复

```
#####五、远程仓库
```
创建ssh key
ssh-keygen -t rsa -C "i@lr.cool"

把公钥id_rsa.pub加到github SSH Keys上面

在github创建仓库，复制仓库链接

本地仓库运行命令
git remote add origin https://github.com/liyuanrui/coding

推送本地内容到远程
git push -u origin master
-u参数是把本地master分支和远程master分支关联起来，以后简化命令

远程库克隆本地库
git clone https://github.com/liyuanrui/coding

本地推送到远程命令
git push origin

本地拉取远程命令
git pull origin

```