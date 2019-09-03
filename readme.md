Android studio 怎么连接安卓模拟器呢，跟着下面的步骤即可
（以雷电模拟器为例，其他模拟器类似）

### 一、下载模拟器
下载安装完雷电模拟器，打开并进入如下页面 
![雷电模拟器桌](https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-1.png)

### 二、模拟器进入开发者选项，勾选usb调试
点击桌面系统应用—>打开设置—>连续点击5次关于平板电脑，会出现开发者选项—->进入开发者选项—->勾选usb调试。
![设置开发者选项](https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-2.png)
### 三、连接模拟器和android studio
按win+r，输入cmd打开命令控制器，将目录切换到你安装雷电模拟器的文件夹下，我安装模拟器的目录如下：
```
Y:\>cd y:\Changzhi\dnplayer2
```
![进入模拟器的目录]https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-3.png)
接下来，雷电模拟器的adb连接端口可以是（5555+index*2）（index>=0）即5555，5557，5559等等（其他的模拟器看下面）
```
y:\Changzhi\dnplayer2>adb.exe connect 127.0.0.1:5555  
```
![连接成功](https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-4.png)

这里很重要，不同的模拟器对应的端口不同，别的模拟器端口请看：
> 夜神模拟器：adb connect 127.0.0.1:62001 
逍遥安卓模拟器： adb connect 127.0.0.1:21503 
天天模拟器：adb connect 127.0.0.1:6555 
海马玩模拟器 ：adb connect 127.0.0.1:53001 
网易MUMU模拟器：adb connect 127.0.0.1:7555

### 四、打开android studio

### 五、run Android studio的项目
执行完上面的指令后，把我们的android studio里面的示例代码run起来，就会收到模拟器的连接信息，点击ok
![](https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-5.png)
然后会出现下面这个提示框
![](https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-6.png)
左边按钮为安装本地模拟器，但是本地模拟器启动比较慢且占用内存。我们选择右边按钮，就可以看到我们的示例在雷电模拟器跑起来了。

![](https://github.com/MengYingjie/AndroidStudio-SDK/blob/master/19-7.png)
至此，连接完毕。


>遇到此类问题，但看了文章还是不懂，
可以加我的qq交流一下，我一定尽全力解答
QQ：781378815
[·个人网页·](http://www.mengyingjie.com/)   [·微博·](https://weibo.com/5172374413/profile?rightmod=1&wvr=6&mod=personinfo/)   [·豆瓣·](https://www.douban.com/people/185977129/)    [·知乎·](https://www.zhihu.com/people/meng.yingjie/activities)[·Instagram·](https://www.instagram.com/meng.yingjie/)  [·Facebook·](https://www.facebook.com/myj.mengyingjie)   [·Twitter·](https://twitter.com/MengYingjie)  
