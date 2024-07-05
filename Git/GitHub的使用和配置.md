![[Pasted image 20240703235047.png]]右上角搜索界面，输入linux后，选择最上面一个点进去如下
![[Pasted image 20240702102747.png]]![[Pasted image 20240702103124.png]]右上角 code可以克隆或下载这个仓库
![[Pasted image 20240702103321.png]]
左上角是分支和tag
![[Pasted image 20240702103343.png]]
右边是仓库的概要信息：发布的版本数，贡献者，使用的主要语言
![[Pasted image 20240702103408.png]]
点击左上角猫脸回到主页
![[Pasted image 20240702103542.png]]
点击New repository创建仓库
![[Pasted image 20240702104920.png]]
![[Pasted image 20240702105105.png]]输入相关信息后，点右下角创建
仓库主页面如下
![[Pasted image 20240702105202.png]]https开头的这种方式在我们把本地代码push到远程仓库的时候，需要验证用户名和密码
![[Pasted image 20240702105433.png]]而git开头的这种方式使用的是SSH协议，这种方式在推送的时候不需要验证用户名和密码，但是需要在GitHub上添加SSH公钥的配置，更安全方便
![[Pasted image 20240702105559.png]]
复制仓库地址，git clone 仓库地址，报错没有正确访问权限。因为使用SSH方式必须配置SSH密钥

![[Pasted image 20240702110016.png]]**ssh-keygen（generate） -t 指定协议 -b 字节大小**
![[Pasted image 20240702110206.png]]![[Pasted image 20240702110448.png]]![[Pasted image 20240702110504.png]]在路径.ssh下，否则默认为id_rsa，输入路径文件名test
![[Pasted image 20240702110707.png]]
输入密码为空，完成创建
![[Pasted image 20240702110900.png]]没有拓展名的test是私钥文件，谁也不要给
有拓展名.pub的是公钥文件，上传到GitHub![[Pasted image 20240702110958.png]]![[Pasted image 20240702111014.png]]
打开公钥文件，全选，复制（命令模式下鼠标全选直接ctr+c，不用讲前面的标识1也选了）到，回到Github界面点击右上角头像，点击Settings，
**注意：复制密钥时，SSH公钥的正确格式时一行完整的字符串，没有多余的空格换行，可以送给gpt改一下再复制到相应key中，否则大概率会创建失败**
![[Pasted image 20240702113412.png]]

![[Pasted image 20240702111353.png]]![[Pasted image 20240702111637.png]]![[Pasted image 20240702111730.png]]
点击SSH and GPG keys
![[Pasted image 20240702111849.png]]![[Pasted image 20240702111854.png]]
点击绿色
![[Pasted image 20240702111941.png]]
把刚刚复制的公钥内容粘贴到key中的输入框，标题Title任意输入，点击下面绿色  添加SSH密钥 这个按钮
![[Pasted image 20240702112129.png]]成功把SSH密钥添加到Github上
 ![[Pasted image 20240702113201.png]]
 因为当时创建密钥选了/.ssh下的test路径，最后需要添加5行配置文件，配置文件意思是：当我们访问github.com时，指定使用SSH下的test这个密钥![[Pasted image 20240702114119.png]]tail显示文件末尾内容
![[Pasted image 20240702114602.png]]与上面视频中创建的核心基本一样![[Pasted image 20240702115225.png]]![[Pasted image 20240702115429.png]]![[Pasted image 20240702115635.png]]![[Pasted image 20240702115652.png]]重新克隆，点进去蓝色即可看到原来的URL网址。git clone 网址
![[Pasted image 20240702120400.png]]![[Pasted image 20240702120310.png]]仅在本地仓库有hello.txt，但是github上的远程仓库还是空的![[Pasted image 20240702120641.png]]
本地和远程相互独立，同步机制如下：
拉取pull，推送push
 ![[Pasted image 20240702120836.png]]推送后，刷新github即可发现同步![[Pasted image 20240702120953.png]]![[Pasted image 20240702121041.png]]![[Pasted image 20240702121052.png]]![[Pasted image 20240702121056.png]]
 