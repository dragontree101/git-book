# git-book

添加远程仓库的一个别名
git remote add <shortname> <url>
git remote add origin git@github.com:dragontree101/git-book.git

推送本地的master分之到origin的master分支
git push -u origin master

查看远程仓库的详细信息命令
git remote show [remote-name]
git remote show origin

你想让文件保留在磁盘,但是并不想让 Git 继续跟踪。当你忘记添加 .gitignore 文件,不小 心把一个很大的日志文件或一堆 .a 这样的编译生成文件添加到暂存区时,这一做法尤其有用。为达到这一目 的,使用 --cached 选项:
git rm --cached log1.log（把加入git管理的log1.log移除出git，并且保留该文件在当前目录）


git上面直接进行mv操作：运行git mv就相当于运行了下面三条命令:
mv README.md README
git rm README.md
git add README


git reset HEAD <file>
取消暂存的文件

git checkout -- <file>
撤销对文件的修改（文件还在没有被纳入到暂存区）

检出一个标签
git checkout -b [branchname] [tagname]
git checkout -b  v1.0.2   v1.0.2

git checkout -b version3
git push -u origin version3
