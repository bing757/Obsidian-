![[Pasted image 20240705081735.png]]![[Pasted image 20240705082024.png]]
- 当前两分支的最近共同祖先：main3，
- 如果在dev分支，就将dev当前所在文件到main3之间的文件合并到main分支
- 在main分支，同理合并到dev分支中
![[Pasted image 20240705082338.png]]
- git branch -d 分支名，删除
- git checkout -b 分支名，创建并切换，后面加id参数（从graph命令可以查看，因为使用了alias定义了别名）可以创建当前id（即commit_hash)时的分支状态并切换，类似与恢复某一状态。如果恢复的不是某一删除的分支，可以直接用git checkout commit_hash或者git reset --hard commit_hash
![[Pasted image 20240705084352.png]]
（上图前面已经删除了feat分支，防止干扰）
- 再切换到main分支，恢复与dev合并前的main5文件
![[Pasted image 20240705084728.png]]![[Pasted image 20240705084805.png]]
- 拷贝两份branch-demo以演示不同rebase操作
![[Pasted image 20240705084943.png]]
- 打开rebase1文件夹：
![[Pasted image 20240705085524.png]]
![[Pasted image 20240705085942.png]]
- 上图，在dev分支中git rebase main，dev分支会编程一条直线，将dev分支中的那一段加在main分支顶部
- 而main分支自己没有变化，因为没有在main分支上执行合并变基操作
- 注意这个alias命令只在当前终端会话中有效。如果关闭终端，或者打开一个新的终端，这个别名就不再有效
![[Pasted image 20240705090934.png]]
 ![[Pasted image 20240705091016.png]]
 ![[Pasted image 20240705091054.png]]
 - 当前分支的 branch out 节点是指这个分支从其父分支的哪个提交点开始分支出来的。
 - rebase适用于自己使用，公共场合协作工作使用merge，整体而言还是使用merge
 ![[Pasted image 20240705092645.png]]