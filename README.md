<div align="center"><a href="http://pvpin.com"><img src="https://dn-coding-net-production-static.qbox.me/3113aa7b-291d-402e-819e-bebbf07e5ef3.png"></a></div>
 

__用拼积木的方式开发Minecraft插件__


__Developing Minecraft plugins by building blocks like playing kids' game.__

 ##### Please note the PVPIN's blocks are based from the [Google Blockly](https://github.com/google/blockly).
 

## 介绍 

#### introduce

### Pay attention 

All English text in this README are not so well, because this just used machine translation. If you're not really understand that all, I'm hope you can forgive me, and, if you can help me to improvement this, that I will thank you. [Well, click here to help me](mailto:i@timewk.cn).

#### Improvementer, maybe

[Dobby233Liu](https://github.com/Dobby233Liu)
 
### 这是什么 
##### What is this?

这是*PVPIN*，一个基于JavaScript实现编写Java语言用于“我的世界”/“Minecraft”中的Bukkit服务端插件的一个网站使用的中等运行环境时(也就是前端)的源代码。

This is *PVPIN*, based on JavaScript to write some Java code and using in the Minecraft's Bukkit server plugins, and this is the orignal runtime source. 


#### 为什么可以使用JavaScript开发Java版的Minecraft插件？
##### Why we can use JavaScript to develop Java version of the Minecraft plugins?

因为Java运行环境中有一个JavaScript引擎，可以运行JavaScript代码。更重要的是，可以直接在JavaScript中调用Java代码。这样，我们就可以用JavaScript来写“Java”程序。

Because the Java runtime environment have an JavaScript engine, so it can run the JavaScript code. More importantly, you can directly using the Java code in JavaScript. In this way, we can use JavaScript to write "Java" program.

<div align="center"><img src="https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_0.jpeg"></div>

这样做有以下几个好处：

* 更简单，JavaScript是一门比Java更简单的语言。学习更快，编写相同的功能，花费的时间也更短；
* 互用性，因为是互用性语言，JavaScript可以被修改和使用在服务器运行中的代码。
* JavaScript本身是一门性价比高的语言，值得一学。性＝用途广泛性（跨前后端与各种平台），价＝学习的代价（耗费时间与难易程度）

This has the following benefits:
* JavaScript is a more simple language than JAVA. Learn faster, write the same function, and take less time;
* dynamic, as a dynamic language, JavaScript can be modified and deployed in the server running code.
* JavaScript itself is a cost-effective language, it is worth learning. cost = use wide (across the front end and various platforms), price = the cost of learning (time and difficulty)

#### 如何使用它?

##### Pay attention 

This part will not have English text because the *PVPIN* was not really have an English page, only Simplified Chinese seem like can be approved. and, the *PVPIN* is just made for Chinese Minecraft Players. If you really want use *PVPIN* in English, please contact us! We will communicate this thing.                        
You can contact us by QQ or E-mail. But, we have a Copyright statement.

QQ member: 4740281 

Mail: [There](mailto:gangma@foxmail.com) 







(everyone: \*sigh\* the bugin sucks)









在此之前，你需要拥有一个PVPIN账号来编写插件，详细的规则请查看PVPIN内的相关帮助。

一、获取服务端包。

这里有一个简单的整合包：[https://pan.baidu.com/s/1dENjTyL](https://pan.baidu.com/s/1dENjTyL)
		
		
下载后解压：

 ![解压](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_1.png)

我们简要的解释一下压缩包里的这几个目录与文件：

* plugins 目录：这里就是放插件的地方。这里已经放了一个NPC插件 citizens-2.0.21-SNAPSHOT，*PVPIN*的NPC功能直接调用了这个插件。
* server.properties ：这是服务器的配置文件。你可以根据自己的需要修改，然后重启就可以生效。
* start.bat、start.sh  ：这是启动服务的脚本。start.sh是给Mac用的。

双击启动脚本start.bat (前提是你已经安装好了java8)，就可以看到启动消息了。

 ![消息](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_2.png)

同时会发现目录下又多了几个文件，其中最重要的就是world目录。

* world 目录：这样的目录有好几个，都是用world开头的，例如world，world_nether，world_the_end。这里就是存放游戏地图的目录。在游戏运行的时候，最好不要修改里面的文件，有可能会带来严重的错误。

#### 连入服务器

* 打开Minecraft客户端，选择“多人模式”。
* 选择添加服务器
* 填入本地ip（127.0.0.1）
* 然后就可以连入了

![连接1](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_2_1.png)

![连接2](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_2_2.png)

关于开服更详细的介绍请看[czfy和aria的教程](http://bbs.pvpin.com/topic/217)。

#### 如何下载和运行在*PVPIN*上开发的插件？

进入“我的作品”，在每一个作品下，有一个下载jar按钮。（必须要中级会员）

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_3.png)

如果点击后看到了这样的界面：

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_4.png)

说明你的程序里用到了“我”这块积木，或者使用了没有指定出生位置的“建筑精灵”。请不要给导出的代码包含这两块积木，因为在服务器里不知道谁是“我”，而没有指定出生位置的“建筑精灵”，实际上也是取了“我”的位置，所以一样不能使用。

在正常情况下，你会看到这样的界面

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_5.png)

这时你有两个选择，下载jar包或者只下载js文件。如果你没有安装过其他用PVPIN制作的插件，请先下载jar包，因为这里包含了pvpin的js运行环境。

将你下载好的插件放进plugins目录下。

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_6.png)

然后关闭服务器窗口，重新启动。看到PVPIN OK. 说明插件加载成功。

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_7.png)

这时候再看服务器目录，会发现多了一个PVPIN目录，这里包括了pvpin的js运行环境和你自己写的插件。

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_8.png)

我们进入这个PVPIN目录，在 plugins/player 下里面就是你开发的js插件。

![](https://raw.githubusercontent.com/PVPIN/pvpin_js_rt/master/images/jar_9.png)

如果你要安装第二个插件，只需要下载插件的js文件，然后把js放进这个目录，然后重启服务器即可。不需要重新下载jar包，否则可能会覆盖。

至此，本文已经结束。尽情享用吧！

###### 提示：PVPIN的js运行环境会不时更新，请关注网站的更新通知。 


### GPL v2 开源协议


This project uses GPL V2 open source protocol for production, please follow this agreement in the relevant operations!

If it is for commercial use, please declear copyright at the relevant location!

Copyright 2017 PVPIN.com

Thanks again for your reading!

		
