命令行解释器，接受用户输入命令，调用操作系统内核执行这些命令，再把执行结果返回给用户
![[Pasted image 20240629103022.png]]![[Pasted image 20240629103516.png]]![[Pasted image 20240629103324.png]]$0表示当前正在执行的脚本文件名称，可以更改。
$SHELL表示整个环境变量所使用的默认脚本文件名称，一般不会更改
![[Pasted image 20240629103445.png]]
创建脚本
![[Pasted image 20240629104001.png]]
i模式下输入如下#！//表示这个脚本文件使用的是bash解释器![[Pasted image 20240629103825.png]]
who am i表示用户名![[Pasted image 20240629104159.png]]![[Pasted image 20240629104425.png]]
bash可以直接执行，./需要添加执行权限
![[Pasted image 20240629105512.png]]脚本中：
![[Pasted image 20240629105859.png]]export命令将变量转换为环境变量，使脚本可用，但仅当前shell，exit再登录就不行。否则name,channel只在当前shell有效!![[Pasted image 20240629110809.png]]
永久有效考虑配置文件（当前用户家目录下）
.profile在用户登录时执行且只执行一次
.bashrc在每次打开一个终端或新建一个会话执行（推荐）
![[Pasted image 20240629110649.png]]
nano .bashrc后鼠标滚动到文件最后面，加上最后两行后保存退出
![[Pasted image 20240629111336.png]]
#注： 修改.bashrc后需要用source或.更新一下
![[Pasted image 20240629111514.png]]
对所有用户都有效的根目录下配置文件
![[Pasted image 20240629111139.png]]将命令的输出结果嵌入到另一个命令或者语句中，需要用命令替换语法
![[Pasted image 20240629114629.png]]

![[Pasted image 20240629114804.png]]fi表示结束if语句
![[Pasted image 20240629114859.png]]![[Pasted image 20240629115313.png]]注意bash语法：if的中括号里语句最左和最右边都得留一个空格
![[Pasted image 20240629115528.png]]加上循环 while do done
![[Pasted image 20240629115909.png]]while true中使用continue和break
![[Pasted image 20240629121219.png]]![[Pasted image 20240629121449.png]]![[Pasted image 20240629121626.png]]![[Pasted image 20240629121702.png]]![[Pasted image 20240629122216.png]]![[Pasted image 20240629120201.png]]
for循环
${fruits[@]}": 表示展开数组 fruits 中的所有元素
![[Pasted image 20240629120326.png]]