fork的使用说明
===
![]()
# 一、Fork项目
### 说明：Fork相当于把别人的项目仓库变为自己的项目，然后你自己可以自由修改，提交到自己的远程仓库。也可以通过的 Pull Request 把你的更改提交回原仓库。

## 1.首先找到要fork的项目，以本测试项为例，点击这个库的Fork按钮创建叉作为自己的项目。
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/Fork.png)
## 2.创建成功后可以在自己的库里找到刚刚Fork的库，注意Fork库的图标是一个叉子
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/forkchuangjian.png)-->
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/kuming.png)
## 3.克隆库到本地做修改。首先复制刚刚Fork下来的项目库地址，注意使用SSH即黄色框里如果显示Use SSH则点击它切换成SSH，如果不是则不需要更改。点击红框图标复制。
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/clone.png)
## 4.在本地新建一个文件夹用作存放克隆的库，然后右键打开gitbash输入
>	$ git clone "粘贴刚刚复制的地址"，
然后回车，等待克隆完成。

---

# 二、分支内容的增加
## 1.修改项目文件，我们先做一个学号名字文件文件并上传合并，打开项目中的name文件夹，新建一个文本文件，输入你的学号姓名
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/wenjianjia.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/name.png)
## 2.接下来要把你修改的信息上传，在forktest文件夹中右键打开gitbash，输入
- $ git add .
- $ git commit -m '备注信息'
- $ git push -u origin master

## 3.登录你的GitHub，提交修改给原作者。首先进入你刚刚fork的库，点击Pull requests
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newFork1.png)
## 4.点击new pull requests
* ![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newfork2.png)
## 5.注意红框中的是你fork下来修改的库名，黄框是原作者的库名。注意主从顺序，我们是要提交到原仓库，所以应该是（从-->主）；确认无误后点击Create
* ![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newfork4.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newfork3.png)
## 6.填入文档说明，然后点击Create Pull requests，显示提交成功，接下来只需要由我确认合并你修改的文件就能显示在此项目中了。
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/fork5.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/fork6.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/ok.png)

----

# 三、分支内容修改和删除
## 1.对fork的内容进行操作前，需要保持库为最新版本，先更新自己的分支，因为要从主仓库更新所以逻辑顺序是(主-->从)
* 先点击New pull request进入拉取请求界面![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/xiugai/1.png)
* 注意如果没有分支选项先点击compare across forks
* 红色框里是主仓库文件，黄色框是你自己的Fork库文件，注意顺序，然后输入备注和说明一路点击绿色按钮提交完
* ![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/xiugai/2.png)
## 2.进入你的本地库文件夹，右键gitbash从github上快速合并更新代码
- $ git pull origin master
## 3.进行你的修改操作，完成后重复第二条的步骤并提交，通知我确定合并以后即可完成主仓库更新。

---