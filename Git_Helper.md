###Git使用小教程
###一、浅谈版本控制
由于现代的互联网行业，普遍是多人分工完成一个项目，那么，如何将去管理多个人共同写的代码呢，于是人们发明了版本控制工具。版本管理工具允许人们将本地的文件同步至版本控制服务器，也允许从服务器将其它人的文件拉下来，其实你也可以把版本控制理解为一个多人共用的网盘（当然实际上比网盘强大的多）。

目前主流的版本控制工具有两种：SVN和Git，一般来说较传统的公司会用SVN，较新潮的公司会使用Git，关于这两者的区别见：http://blog.csdn.net/bruce_6/article/details/38299677

由于煎饼计划的代码均需上传至github，我就以Windows平台下的TortoiseGit为例将下git的几个基本命令，当然学会了TortoiseGit，再学TortoiseSVN也很容易。
###二、注册GitHub账号
1.注册
在使用Git前，首先你要有个Git服务器，目前用的最多的免费git仓库是GitHub，注册地址是：https://github.com/join
2.权限的开通
光有账号是不行的，你还需要相应的读写权限，想开通煎饼计划的git，请联系陶陶为你开通权限
3.接受邀请
陶陶邀请你后，你会收到一封邮件，点击同意即可开通
没收到邮件的，访问下https://github.com/wuanlife，页面顶上会有相关的通知
###三、TortoiseGit的基本操作
####1.安装
在安装TortoiseGit前我们需先安装Git主程序，下载地址为：https://git-scm.com/downloads ，下载后一路next安装就可以。
安装完Git，我们再去下载TortoiseGit，下载地址为：https://tortoisegit.org/download/ ，分为32位版和64位版，下载时要选好，安装的时候也是一路next。

官方地址无法下载的，可以去网盘下载：http://pan.baidu.com/s/1sj9rsex 密码: 4jmg
####2.Clone
例如午安煎饼计划PHP组的Git地址是：https://github.com/wuanlife/Jianbing_PHP.git ，前端组的Git地址是：https://github.com/wuanlife/Jianbing_Web.git ，UI组的Git地址是：https://github.com/wuanlife/Jianbing_UI.git ，复制下来。

然后打开硬盘里的一个目录，最好是专门开发用的目录，点右键，选择“Git Clone...”，将地址复制进去，点击OK，如图：

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_1.png)

出现Success提示，就代表clone成功了，close掉对话框，然后就出现了名为Jianbing_PHP的文件夹了。

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_2.png)
####3.Commit
commit代表提交版本操作，即为将你的本地改动保存为一个版本，我们以新建文件为例。

首先，我们打开刚才生成的Jianbing_PHP，新建一个文件夹，例如Taotao，再到这个文件夹里建一个名为readme.txt的空文件。

然后我们在这里点击右键，选择Git Commit -> "master"...，弹出如下对话框，

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_3.png)

上方的Message即为本次提交版本的改动内容，如“新增readme文件”，同时因为新增的文件是默认不被选中的，我们还要手动选中readme这个文件，然后点击OK

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_4.png)

出现Success提示，就代表提交成功了，同样close掉对话框。此时你可以接着在本地改动，继续commit。一般来说，完成一处功能改动或者解决一个bug就可以提交一次。

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_5.png)
####4.Push
commit虽然是提交版本，但是此时你的代码还没同步到服务器，若想同步到服务器，还需要进行push操作。

具体步骤是，在文件夹点击右键，进入TortoiseGit菜单，选择“Push...”，在弹出的对话框中选OK，

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_6.png)

然后输入你在github注册的账号和密码，前提是你要有这个git仓库的write权限

![](https://raw.githubusercontent.com/wuanlife/Jianbing_Wiki/master/image/git_7.png)

出现Success提示，就代表push成功了，同样close掉对话框。打开https://github.com/wuanlife/Jianbing_PHP ，是不是多了个Taotao的文件夹~
###四、其它操作
Git的强大远远不止上面那几个功能，常用的还有pull、revert等操作，更多内容可以看这篇教程：http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000
