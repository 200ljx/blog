# 基本操作
2. 1. git init
2. git add
3. git commit -m 'xxx'
4. git status
5. git diff 文件名    //查看差异，更新也是  add和commit两步
6. git log             //  --pretty=oneline美化日志    --graph --pretty=oneline --abbrev-commit分支合并图
7. git reset --hard 版本号      //HEAD当前版本   HEAD^上个版本    ...   HEAD~100
8. git reflog
9. git checkout -- 文件名       //撤销到更改前
10. git rm 文件名

---
# 分支
1. git branch 分支名         //创建分支
2. git checkout 分支名    //切换分支
3. git branch              //查看分支
4. git merge 分支名          //合并分支
5. git branch -d 分支名       //删除分支
6. git checkout -b 分支名      //创建加切换
7. git branch --set-upstream branch-name origin/branch-name  //建立本地分支和远程分支的关联
8. git stash    //保存工作现场
9. git stash apply  和  git stash pop(同时删除stash)  恢复工作现场

---
# github
1. ssh-keygen -t rsa -C "youremail@example.com"    //创建SSH Key
2. 生成文件id_rsa.pub中的内容 设置到github网站
3. ssh -T git@github.com                  //测试是否验证成功
4. git remote add origin git仓库地址       //与本地库关联
5. git push -u origin master          //推送本地到远程   -u将本地master与远程master关联
6. git clone git远程仓库地址
7. git remote -v  查看远程库信息

---

参考：<a href="http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000" target="_blank">廖雪峰老师git教程</a>