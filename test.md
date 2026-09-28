测试 git add -p [文件名]
-p 参数只能够审查到改变的文件，不能审查到新创建的文件

要先执行  git add -N [文件名] 来告诉 git 开始跟踪这个新文件，**注意并没有将这个文件加入暂存区**

要指定加入某一个文件可以用 git add <pathname>

````git
git add test.md test1.md
````



git commit -m "添加信息"
git commit --amend --no-edit 漏加文件或写错信息？吸纳暂存区并重写上一次 commit（不产生新节点）

**主要是用来进行一次 commit 后还没有 push 的情况下进行文件的追加，但是这次追加是漏的**


git diff 判断*工作区和暂存区*的对比，会将工作区的文件和暂存区的文件进行对比，比较修改了哪些内容 **如果是新建的文件，没有添加到暂存区的时候，是不会显示出来的**

git diff --staged 判断*暂存区和本地库*的对比

git  diff HEAD 判断*工作区和本地库*的对比