![[Pasted image 20240702201733.png]]
应该在.ssh下使用ssh-keyget,下图路径是错误的，会被修改，使用mv指令修改路径，相当与 ctr+x
![[Pasted image 20240702211105.png]]
![[Pasted image 20240702205643.png]]![[Pasted image 20240702205839.png]]
在.ssh下的配置文件中添加和之前github相同的配置形式
![[Pasted image 20240702205920.png]]
![[Pasted image 20240702210145.png]]
**注意：gittee上的密码是账号密码（11位），下面的passphrase for key / / / / testgitee才是创建公钥ssh-keygen设置的123**
![[Pasted image 20240702223121.png]]
![[Pasted image 20240702222757.png]]![[Pasted image 20240702223309.png]]
测试成功，不测试也可。
**ssh-keygen后，公钥和config配置好后，即可git clone和git push**
创建仓库
![[Pasted image 20240702223742.png]]![[Pasted image 20240702223827.png]]
克隆正常，成功![[Pasted image 20240702223949.png]]
鼠标靠近gitlab左侧，换出用户相应菜单
 鼠标放在可壁纸和页面连接处
 ![[Pasted image 20240702230831.png]]
 ![[Pasted image 20240702231101.png]]密钥密码是tangshan
 ![[Pasted image 20240702231120.png]]![[Pasted image 20240702231136.png]]![[Pasted image 20240702231223.png]]![[Pasted image 20240702231527.png]]
 ![[Pasted image 20240702232443.png]]
git remote add 远程仓库别名  远程仓库url，增加本地仓库my-repo关联的远程仓库，现在他同时关联了公有的Github和私有的GitLab 
本地仓库默认关联Github，git push不加参数默认更新到Github。
git push gitlab main分支可以推送到私有的GItLab上![[Pasted image 20240702232717.png]]![[Pasted image 20240702233516.png]]

