默认--mixed
![[Pasted image 20240702084540.png]]   ![[Pasted image 20240702084712.png]]
左上角是未回退版本，将此文件夹cp -rf(递归强制force）3次，分别对三个目录进行回退，ls是工作区，git ls-files是暂存区，HEAD指针指向当前分支
谨慎使用-hard，放弃本地所有修改，删除。若误操作，git reflog查看记录，找到之前的版本号，git reset --hard  版本号,回退到之前版本即可
![[Pasted image 20240702085559.png]]![[Pasted image 20240702090441.png]]