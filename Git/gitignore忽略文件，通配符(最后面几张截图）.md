 ![[Pasted image 20240702092943.png]]![[Pasted image 20240702093635.png]]![[Pasted image 20240702093700.png]]**通配符‘星号’和？***
 ![[Pasted image 20240702093938.png]]
 创建两个.log，将一个.log放入.gitignore,add和commit之后，使用vi
 在.gitigore中加上一行*.log![[Pasted image 20240702094359.png]]
 ![[Pasted image 20240702094555.png]]>>other.log表示在other.log文件后面追加的内容
 因为other.log  commit到版本库后才修改.ignore文件，所以他没有在.ignore中。这时需要先把他从版本库删除再提交，git rm --cached从暂存区删除但工作区保留![[Pasted image 20240702094656.png]] ![[Pasted image 20240702095018.png]]
 .ignore文件如下，文件夹格式以/结尾，这样才能正确忽略文件夹
 ![[Pasted image 20240702095517.png]]
 -s表示short,简短显示status
 ![[Pasted image 20240702095649.png]]重要：
 ![[Pasted image 20240702100341.png]]
 Blob模式表示正则表达式![[Pasted image 20240702095909.png]]![[Pasted image 20240702100017.png]]![[Pasted image 20240702100534.png]]