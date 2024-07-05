**+表示添加权限，-表示删除权限，-rwx**
![[Pasted image 20240629093258.png]]特定添加：u表所有者，g表所在组，o表用户
第二列数字表示链接数，硬链接数
![[Pasted image 20240629093649.png]]
数字表示法：
![[Pasted image 20240629093824.png]]
![[Pasted image 20240629093856.png]]
#windows下以盘符开头，linux以根目录开头
根目录/下ls
![[Pasted image 20240629094543.png]]![[Pasted image 20240629094721.png]]cp表示拷贝，mv表示移动  /重命名文件或目录
rm表示删除，
vi、touch（碰 一下文件，使其修改时间为当前时间，如果此文件不存在则创建文件）、echo "xxx">file可以创建文件![[Pasted image 20240629095132.png]]
makir表示创建目录，-p（parents）表示创建多级目录，第二列表示如下：
![[Pasted image 20240629095414.png]]![[Pasted image 20240629100403.png]]![[Pasted image 20240629100602.png]]![[Pasted image 20240629101202.png]]![[Pasted image 20240629100510.png]]复制目录需要加-r递归
![[Pasted image 20240629101240.png]]
du（disk usage）查看文件大小、目录结构，第一列表示大小
专门显示结构的tree命令
![[Pasted image 20240629101632.png]]
删除目录rmdir只能删除空目录，非空需要rm -r，删除后不可恢复，没有回收站，小心
![[Pasted image 20240629101856.png]]