初始在命名模式，
insert，append，open首字母可进入插入模式，
：尾行模式
![[Pasted image 20240628233854.png]]![[Pasted image 20240628234040.png]]键盘上下左右也可
![[Pasted image 20240628234129.png]]![[Pasted image 20240628234532.png]]
一次操作一行，在命名模式下
2yy：复制两行内容，当前行为第一行，第二行为向下一行
3p：把刚复制的两行粘贴3次
![[Pasted image 20240628235135.png]]：set number回车后可以在左边看到行号，缩写 ：set nu
：set nonumber不显示行号
：27加回车 可调到27行
![[Pasted image 20240628235531.png]]
![[Pasted image 20240628235625.png]]
#查找：
![[Pasted image 20240629000113.png]]向下查找是     ？+ 内容
   上                  / + 内容
按下回车后，输入n表示查找下一个，方向依据？/定
末尾加\c表示忽略不区分查找大小写
![[Pasted image 20240629000814.png]]
#替换
![[Pasted image 20240629001003.png]]
 加上/g可以替换每一行所有匹配到的内容，g表是全局
 ：后面40,50表示替换行范围为【40,50】，如果只在当前行可以省略       注：替换整个文件是1，$
 s表示替换，**Substitute**（替换）
 //表示替换Hello为World
![[Pasted image 20240629001040.png]]
#撤销
命令模式下按 u（undo），相当于ctrl+Z
相当于配置文件：
![[Pasted image 20240629002117.png]]
把习惯的操作写入配置文件中![[Pasted image 20240629002223.png]]![[Pasted image 20240629002633.png]]
![[Pasted image 20240701231528.png]]