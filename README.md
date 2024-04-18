# git

## rebase vs merge

开发feature分支时,如果master有更新,可以使用 git pull --rebase master,推送到远端分支

master合并fearure分支时,使用 git merge --no-ff feature

### 参考

- [因为master不应该用rebase合并，就要停止使用rebase？？？ 我的实践是master合并feature branch时用merge，但如果我在feature branch上要解决和master的冲突，会rebase origin/master 然后再push 提PR](https://zhuanlan.zhihu.com/p/29682134)
- [When should I use git pull --rebase?](https://stackoverflow.com/questions/2472254/when-should-i-use-git-pull-rebase)
