# RPGMakerMV/MZ游戏系列汉化教程

## 创作初衷

末法时代，如今的游戏只有自己去汉化和校对润色，汉化组已死，所以自食其力。

以及对3DM中的RPGMakerMV/MZ游戏解包、解密工具包的补充。因为该工具包禁止转载所以就不发链接了，只需要在3DM mod官网输入rpg就可以看到。

#### 请注意：因为rpg游戏不像renpy那样国内没啥资料，所以这里的汉化教程、加密以及打包教程只是其中一种方法，且本教程基于的是rpgmaker mv/mz的版本关于其他版本如xp vx ace 一律不回答，作者并没有义务回复这些问题。

## 1.如何汉化？

首先你得准备以下工具

Translator++ [下载地址](https://pan.baidu.com/s/1VDu1LBDqYAFXfBIpn-kCDQ?pwd=pay2) 解压码：Dreamsavior

一款rpgMakerMV/MZ做的游戏

### 1.1 架构介绍

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-1.jpg)

这是一个常规的非封包的rpg游戏，如果是封包的rpg游戏正常来讲只会有一个www文件夹和一个game.exe文件或者只有一个exe文件(如Enigma打包或者nw.js)，这种打包法game.exe文件非常大。如果很多文件后缀是rpgmvp、.rpgmvo的话则需要去解密，详情可以去看3DM中的RPGMakerMV/MZ游戏解包、解密工具包。这里不做过多解释。

我们只需要在**www中的data文件**里面去汉化即可。如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-2.jpg)

### 1.2 使用Translator++

这里为了简便将Translator++写为t++

#### 1.2.1 首先打开t++ 选择start a new project

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-03.png)

#### 1.2.2 选择rpgmaker

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-04.png)

#### 1.2.3 选择一个无封包的rpg游戏exe文件，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-05.png)

#### 1.2.4 同时你也可以选择备份，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-06.png)

#### 1.2.5 汉化的数据在data里面而不是在js里面这点不要搞错了

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpgmaker/rpg-07.png)

#### 1.2.6 选取data里面的目录右键点击批量翻译，如图。

![](https://cdn.jsdelivr.net/gh/dclef/CDN/wechat/rpg-09-01.png)

#### 1.2.7 点击设置选择翻译源以及源文本语言和要翻译文本的语言

![](https://cdn.jsdelivr.net/gh/dclef/CDN/wechat/rpg-09-02.png)

#### 1.2.8 等待翻译结束，Abrot是停止，Pause是暂停但窗口不关

![](https://cdn.jsdelivr.net/gh/dclef/CDN/wechat/rpg-10.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-11.png)

#### 1.2.9 这里简单介绍优先级：initial<Machine translation<Better trasnlation<Best translation 如果你默认只翻译了初始翻译导出的时候就是初始翻译，假如四个都翻译了 那么最佳翻译就是导出的翻译 如果有时间你就可以在此润色

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-12.png)

#### 1.2.10 然后选择要翻译的文件右键选择该选项注入翻译，并选择原先的游戏根目录应用即可

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-13.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-14.png)

#### 1.2.11 当然你也可以选择导出文本翻译 然后备份原有目录。如果要测试，则仅需要在备份原有数据的情况下将导出的数据覆盖原有的数据即可

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-15.png)

### 1.3 审查/校对/润色

#### 1.3.1 审查

刚刚机翻完的文本只是初稿，对于运行游戏而言只能说可以运行起，对于大部分游戏而言会有BUG存在，这时候你需要检查是否缺少或多打的正反斜杠、方括号、空格等字符都可能导致游戏无法运行。

#### 1.3.2 校对

最好的方式是先将中文的字符都换成英文字符，避免因为中文字符造成BUG。

至于看不见的BUG你还是需要去运行游戏一遍才能看出哪里出错了。当然RPG的BUG千奇百怪，需要非常细心的排查如果发现BUG实在解决不了可以先忽略这一部分的翻译，然后逐一排查。

#### 1.3.3 润色(人工翻译)

润色对于校对来说就非常简单了，你只需要把看着很奇怪的翻译文本翻译成人话就行，就比如save，机翻可能会叫拯救，这时候你就改翻译成保存。你可以使用deepl进行比较，有些俚语使用deepl可以翻译出来，而不是机翻的直译。当然这不可能跟人相比，只是相比于机翻而言能看一点。

### 1.4 解包

如果你没使用t++，想自己解包的话，请使用Java-RPG-Maker-MV-Decrypter

此前提条件是必须有JAVA的环境，关于如何配置JAVA的环境变量这里不必多说，百度上非常多教程。

下载地址：https://github.com/Petschko/Java-RPG-Maker-MV-Decrypter

###### 如果下载较慢可以关注微信公众号【老猫的杂货店】输入[rpg解包工具]获取

#### 1.4.1 点击start.bat，会显示一个GUI画面，选择File->select RPG MV/MZ project

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-59.png)

#### 1.4.2 如果key存在system.json的话，会如图显示，点击Decrypt->All Files就可以进行解密，然后输出路径在output中，但其中会有一些文件解不出来，这里需要你自己去斟酌

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-60.png)

## 2.使用RMMVCookTool对rpg进行JS加密

前提说明：我并不提倡一个汉化者对一款不是自己的游戏进行加密，假如你对这款游戏写了JS脚本但不想让别人知道，那么这款加密方式适合你。

注意：这里的加密的是rpgmaker MV做的游戏

这个加密方式是将JS转成二进制文件，防止别人获取文件。这里默认修改成bin文件

项目地址:

https://github.com/FirehawkV21/RMMVCookTool
前提条件你得需要一个nw.js的包，一款rpgmaker MV的游戏

下载地址：https://nwjs.io/

##### 你也可在公众号【老猫的杂货店】输入[rpg加密工具]获取下载链接

### 2.1 首先把nw.js sdk导入ROMMVCookTool中，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-15-1.png)

### 2.2 打开www中的index.html文件 更换成如图所示的代码

``![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-16.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-17.png)

代码如下：

```html
<script>nw.Window.get().evalNWBin(null, "www/js/libs/pixi.bin");</script>
<script>nw.Window.get().evalNWBin(null,
        "www/js/libs/pixi-tilemap.bin");</script>
<script>nw.Window.get().evalNWBin(null,
        "www/js/libs/pixi-picture.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/libs/fpsmeter.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/libs/lz-string.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/libs/iphone-inlinevideo.browser.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/rpg_core.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/rpg_managers.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/rpg_objects.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/rpg_scenes.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/rpg_sprites.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/rpg_windows.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/plugins.bin");</script>
<script>nw.Window.get().evalNWBin(null, "www/js/main.bin");</script>
```

### 2.3 在js中的rpg_managers.js找到行数2805附近，这里显示的是2810.将js改为bin，如图。

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-18.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-19.png)

### 2.4 再转到行数2826附近，这里是2830，更换如图所示代码

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-20.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-21.png)

代码如下：

```js
PluginManager.loadScript = function(name) {
    nw.Window.get().evalNWBin(null, "www/js/plugins/" + name);
};
```

### 2.5 当然如果工程被rpgmaker加密过你还可以进行进一步加密(可跳过忽略)，找到data中system.json的密钥，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-22.png)

### 2.6 删除并复制system.json中的密钥，打开rpg_core.js，找到行数9256，找到如图所示代码并将密钥粘贴上去进行代码更换，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-23.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-24.png)

### 2.7 再转到行数147附近，找到如图所示代码，并进行代码修改，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-25.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-26.png)

### 2.8 然后导入游戏根目录，点击compile，勾选porject setting中的remove js，如图，你会看到多了一些bin文件，这便完成了加密(建议先把js文件备份)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-27.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-29.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-28-1.png)

### 2.9 然后将www中的package.json复制到nw.js根目录中并将路径修改成www，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-31.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-31-2.png)

### 2.10 复制www到nw.js，如果能打开说明加密成功。

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-30.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-32.png)

##### 这里如果觉得加密比较麻烦可以关注微信公众号【老猫的杂货店】输入【rpg加密文件】即可获取2.1-2.5步骤修改的index.html和rpg_manager.js文件

## 3.部署打包

### 3.1 使用Enigma Virtual Box封包

实际上用原有的rpgmaker MV部署就已经算打包了，但里面文件可能较多，其次作为汉化者里面的json文件容易被人修改导致被倒卖，所以做一个简单的封包是有必要的，当然如果有钱的话可以使用The Enigma Protector打包，更不容易破解

下载地址：https://www.enigmaprotector.cn/cn/downloads.html

##### 如果下载慢的话可以关注微信公众号【老猫的杂货店】输入【rpg封包工具】获取

#### 3.1.1 打开文件，选择language，选择chinese，程序会要求你重启，重启以后就会显示中文

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-33.png)

#### 3.1.2 选择add，添加文件夹，选择游戏根目录，执行封包，封包成功以后只保留boxed文件即可(当然你可以与上一步加密配套)，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-34.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-35.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-36.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-37.png)

### 3.2 打包安卓

如果使用android studio的话，版本建议不要最新版，新版比较奇怪容易出现BUG，建议选择其他版本，这里我用的2020.3.1。

关于安卓打包是比较麻烦的，当然你可以选择使用website 2 apk，但并不推荐使用这个打包，rpg游戏本质是html，打包只是算套壳打包，也就是webview。但使用这个打包可能会有卡顿，本人还是建议用android studio打包，如果实在不会android studio的就使用website 2 APK打包。

#### 3.2.1 使用rpgmaker MV部署安卓文件

如果你使用其他人的rpg游戏那么是没有Game.rpgproject这个文件，请在www文件夹中创建一个Game.rpgproject文件并用文本打开将rpgmaker版本写入进去，这里我写的文本是RPGMV 1.6.2

打开rpgmaker MV点击左上角 文件-部署，点击android，如果你想要加密文件也可以选择加密(一旦加密密钥就在system.json中)，如图所示

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-38.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-39.png)

#### 3.2.2 使用Website 2 APK Builder打包APK

首先打开此软件，右边请配置如图所示规则

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-40-1.png)

请自行写应用名称、应用包名必须是英文，启动画面、图标可自定义。

本地网站目录就是将刚刚部署android的www文件放在这里，如图所示

然后点击生成创建安卓apk，安装即可，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-41-1.png)

备注：刚刚打包使用的密钥是测试密钥，如图你安装的软件报毒请更换密钥，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-42.png)

前提你必须安装jdk8版本并设置环境变量，由于这是过于常见的问题请自行百度

用管理员模式打开CMD 输入以下代码密钥代码

请自行替换以下关键词：

myalias 别名

newkeystore 密钥库文件的名称

yourpassword 密钥库密码

```
keytool -genkey -keyalg RSA -alias myalias -keystore newkeystore.keystore -storepass yourpassword -validity 36000 -keysize 2048
```

下载地址：https://websitetoapk.com/download.html

###### 如果想要汉化版可以关注微信公众号【老猫的杂货店】输入[rpg打包工具]获取

### 3.3 使用android studio打包APK

注意：如果你是首次打包可能会出错，因为下载gradle文件需要挂魔法

环境准备：

官网下载地址：https://developer.android.com/studio#downloads

或者：https://www.androiddevtools.cn/

APK工程下载地址：https://github.com/AltimitSystems/mv-android-client

###### 如果APK工程下载较慢可关注微信公众号【老猫的杂货店】输入[APK工程]获取

#### 3.3.1 打开android studio并打开工程，会先下载gradle中的文件，如果下载成功会显示android，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-43.png)

#### 3.3.2 在app目录中新建个assets目录，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-44.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-45.png)

#### 3.3.3 将打包好的www文件放入assets目录中，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-46.png)

#### 3.3.4 如果要更换名字，请在res目录中找到values.xml修改名字，如图所示

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-48.png)

#### 3.3.5 如果要替换图标，请先使用图标制作工具，制作完成以后修改成如图所示的名称进行替换

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-47.png)

#### 3.3.6 准备完成以后点击Bulid->Build APK，编译debug模式的APK，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-49.png)

#### 3.3.7 编译成功以后可在日志中看见，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-50.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-51.png)

#### 3.3.8 因为bulid apk 是默认的签名，如果我们要修改签名，请选择singed APK，然后创建Keystore文件，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-52.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-53.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-54.png)

#### 3.3.9 请按要求填好信息后，点击OK，密码别忘了后面如图还要用此签名会用到，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-55.png)

#### 3.3.10 然后点击webviewRelease，勾选V1签名，点击finish，如果编译好了以后会在目录中显示，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-56.png)

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-57.png)

至此，安卓打包教程完成。

## 4.FAQ

因为rpg的游戏种类繁多且在国内有很多资料，以及游戏会有千奇百怪的BUG，所以作者只能靠自己的经验来做问题回答，且作者并没有义务回答您的问题，遇到问题请先自己解决

### 4.1 关于游戏安卓打包后会有音频缺失的情况，该如何解决？

因为在项目js文件里的rpg_manager.js代码，它将手机音频改成了m4a格式，而原先的游戏的音频并没有m4a格式，所以我们打包时会报错，出现无法找到m4a文件的错误，这里有有种比较简单的方法。直接添加一个只允许ogg的插件即可

### 4.2 游戏中会有些在手机中操作不了的手段，所以要添加虚拟摇杆，该怎么做？

使用QJ-button插件即可解决，请在rpgmaker mv中的工具-插件管理中选择QJ-button，然后根据自己的需求自定义按钮，这里要注意的是rpgmaker的键盘似乎跟我们有所差别，这里可以在rpg_core.js看到，如图

![](https://cdn.jsdelivr.net/gh/dclef/CDN/rpg/rpg-58.png)

### 4.3 为什么签名打包APK的时候会有四个选项，按道理说不应该是两个吗？

因为此项目是做了个webview和crosswalk两种选择，crosswalk是谷歌内核，就跟腾讯的x5内核一样，用于提升性能的，你也可以选择此选项，但会多出几十MB的内存

### 4.4 请在github上提交issues，问题会根据issues中的问题或者其他平台反馈的问题持续更新.........

###### 插件关注微信公众号【老猫的杂货店】输入[rpg插件]获取

## 5.参与本github项目

这里本人沿用上一篇文章的图片，本质是一样的操作

如果你只想单纯的提出问题请提交即可，如果你本身有代码基础或者无基础想参与到本项目中并修改机翻的话，请看以下步骤。

### 5.1 git 的安装与使用

下载[git](https://git-scm.com/downloads)，下载完成以后安装到本地(网上搜一下安装教程，这里就不多解释)。

安装完成后，在开始菜单里找到“Git”->“Git Bash”，弹一个类似命令行窗口的东西，就说明Git安装成功

接着需要设置一下信息，这台机器上的所有Git仓库都会使用这个配置 （步骤可以省略）

```
$ git config --global user.name "username"
$ git config --global user.email "email@example.com"
```

### 5.2 vscode中git的使用

安装vscode，默认你已经注册了github账号，请fork我的项目，为了便于理解，这里新创建了一个账号，如图所示

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-12-46.png)

fork完成以后，便会直接跳转到你的仓库，如图所示。

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-18-30.png)

注意：如果项目更新，你需要点击Fetch upstream来更新你的项目，如图所示。

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-22-21.png)

打开你的vscode，新建一个文件夹到你的工作区，选择要放入项目的文件夹中，右键在集成终端中打开，请输入git clone代码，如图所示

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-26-49.png)

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-26-30.png)

代码如下

```
git clone 你的git链接
```

clone完成以后，修改你想要汉化文本或添加你要翻译的文本文件。这里仅演示修改文件。

修改完以后请点击左侧第三个按钮，如图所示

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-33-55.png)

如果首次同步更改会让你去登陆github，如图所示

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-34-36.png)

会出现允许打开url，如图所示

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-35-38.png)

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-35-10.png)

打开并返回到vscode即可成功更新

### 5.3 在你的项目主页中提交request

如果你完成了很多代码修改，请提交一个request，请求合并，如图所示

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-45-45.png)

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-46-33.png)

![](https://cdn.jsdelivr.net/gh/Dclef/CDN/renpy/renpy_2022-01-31_00-47-39.png)

**注意：标题以及内容请说明清楚，否则不会合并请求。**

## 6.尾声

rpgmaker MV/MZ游戏汉化教程(其实重点是MV教程)到这里完结了，常见问题后续会在github上更新，感谢你看到最后！就如我上篇renpy汉化教程一样，也希望你们参与本项目，将翻译文件作为协同翻译，这样人人为汉化游戏出一份力！

同时欢迎关注微信公众号【老猫的杂货店】

如果该项目对你有帮助，可以请我喝杯咖啡。
![](https://cdn.jsdelivr.net/gh/dclef/CDN/renpy/Snipaste_2022-05-01_22-32-56.png)