# git

## rebase vs merge

开发feature分支时,如果master有更新,可以使用 git pull --rebase master,推送到远端分支

master合并fearure分支时,使用 git merge --no-ff feature

[好处](./git-rebase.md)

## rebase

git rebase 命令会将本地分支的提交暂存起来，然后将远程分支的提交拉取到本地，并将本地提交逐个应用到远程分支的提交上。这个过程可以避免出现不必要的合并提交，使得分支历史更加清晰。
git pull 命令会将远程分支的提交拉取到本地，并自动进行一次合并操作。如果本地分支与远程分支有冲突，需要手动解决冲突并提交合并结果。

### 参考

- [因为master不应该用rebase合并，就要停止使用rebase？？？ 我的实践是master合并feature branch时用merge，但如果我在feature branch上要解决和master的冲突，会rebase origin/master 然后再push 提PR](https://zhuanlan.zhihu.com/p/29682134)
- [When should I use git pull --rebase?](https://stackoverflow.com/questions/2472254/when-should-i-use-git-pull-rebase)
