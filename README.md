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
- $ git add 
- $ git commit -m '备注信息'
- $ git push -u origin master

## 3.登录你的GitHub，提交修改给原作者。首先进入你刚刚fork的库，点击Pull requests
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newFork1.png)
## 4.点击new pull requests
* ![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newfork2.png)
## 5.注意红框中的是你fork下来修改的库名，黄框是原作者的库名。确认无误后点击Create
* ![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newfork4.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/newfork3.png)
## 6.填入文档说明，然后点击Create Pull requests，显示提交成功，接下来只需要由我确认合并你修改的文件就能显示在此项目中了。
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/fork5.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/fork6.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/ok.png)

----

# 三、分支内容修改和删除

## 1.首先进入要进行操作的文件夹位置(forktest文件夹)，右键打开gitbash，更新原始库，输入：
* $ git remote add upstream git@github.com:lnkDrop/forktest.git
* $ git fetch upstream

## 2.在本地做出修改，完成后提交到你自己fork出来的项目主页上，输入
* $ git commit -m '备注信息'
* $ git push "fork出来的地址(第一条第3点中的地址)"

## 3.在Github上向原作者提交更改请求，打开fork的项目，在项目主页点击new pull request,就会出现如图所示的图标，点击绿色图标按钮，添加修改描述，提交成功后只需要等待主开发者去合并就可以了。
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/qingqiu.png)
![](https://raw.githubusercontent.com/lnkDrop/forktest/master/img/tubiao.png)


