![[Pasted image 20240701233818.png]]
注意：git commit只会提交暂存区的文件，而不会提交工作区文件
![[Pasted image 20240701234718.png]]
fi
![[Pasted image 20240702001151.png]]![[Pasted image 20240701234325.png]]![[Pasted image 20240701234510.png]]file2没有git add到暂存区，git commit只讲file1提交到仓库![[Pasted image 20240701234750.png]]![[Pasted image 20240701234848.png]]![[Pasted image 20240701235412.png]]
添加参数-m（message）的原因：
![[Pasted image 20240701235738.png]]![[Pasted image 20240701235759.png]]![[Pasted image 20240702000022.png]]![[Pasted image 20240702000314.png]]![[Pasted image 20240702000338.png]]![[Pasted image 20240702000418.png]]![[Pasted image 20240702000440.png]]git commit 不加-m参数进入详细的提交信息界面
在首行i模式输入信息，esc后：wq
![[Pasted image 20240702000621.png]]git log查看提交日志：
commit后面16进制字符串是唯一提交ID
作者，邮箱，日期，message
![[Pasted image 20240702000810.png]]
![[Pasted image 20240702001008.png]]