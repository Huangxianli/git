测试 git add -p [文件名]
-p 参数只能够审查到改变的文件，不能审查到新创建的文件

要先执行  git add -N [文件名] 来告诉 git 开始跟踪这个新文件，**注意并没有将这个文件加入暂存区**

要指定加入某一个文件可以用 git add <pathname>

```git
git add test.md test1.md
````



git commit -m "添加信息"
git commit --amend --no-edit 漏加文件或写错信息？吸纳暂存区并重写上一次 commit（不产生新节点）