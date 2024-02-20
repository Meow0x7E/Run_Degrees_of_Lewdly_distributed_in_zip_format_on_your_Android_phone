# 在安卓手机上运行以zip格式进行分发的《Degrees of Lewdly》

## 汉化相关

汉化的发布仓库是 [Degrees-of-Lewdity-Chinese-Localization](https://github.com/Eltirosto/Degrees-of-Lewdity-Chinese-Localization)

通过阅读汉化仓库的 README，你可以学会怎么安装汉化和图片资源包。你可以在该仓库里获取最新版的汉化 Mod 和构建好的 Modloader。

如有任何关于汉化问题问题，请先熟读并背诵汉化仓库的 README 全文，然后去看看 Issues 里有没有相同问题再发问。***(关注 `Open` 状态 Issue 的同时不要忘了那些已经处于 `Closed` 状态的 Issue)***

发问前请阅读 [提问的智慧](https://lug.ustc.edu.cn/wiki/doc/smart-questions) 以提高你的问题被注意和回答的可能性。

请记住，礼貌永远能让人更乐意耐心解答你的问题，礼多人不怪。

你可以在 [Releases](https://github.com/Eltirosto/Degrees-of-Lewdity-Chinese-Localization/releases) 处获取 DoL 的 Modloader 以及图片资源包和汉化 Mod

## 方法一(简单但不一定有效，Android 12 及以上似乎有限制)

## 可能的问题

来自群友 `652292986` 的话

> 安卓12还是13开始，以及新版本的chrome等浏览器已经拒绝给浏览器分配自身文件夹以外的读取权限了

> 还有就是file://＋文件地址的访问输入的坑也没有提到

> 浏览器你直接输进去回车大概率直接给你搜索了

> 目前用的所有chrome内核系的浏览器都无法直接用回车访问file协议，会直接变成搜索

> 需要用复制全协议＋地址的方法，让地址栏提示访问文件索引

***注意，以上的话我唯一验证过的是file://协议确实有可能无法访问，但不是所有都不可以访问，你可以试试换成别的浏览器，或者试试备用步骤***

实在不行试着催一下我把方法二写了(邮件有延迟，我注意到的时候可能过去一段时间了

### 开始之前

请注意，本教程只负责教你如何安装和打开 `Degrees of Lewdly` ***(在下文里简称 `DoL`)*** ，汉化和美化的安装并不包括在内。

当你看到 :monocle_face: 时，如果你对当前文本感到不解或者不知道怎么做的时候，请去使用浏览器搜索。因为这只是一篇简易教程，所以不会开太长篇幅讲和目标无太大关联的东西。

这里我有一个个人建议，使用bing或其他国外搜索引擎作为你搜索问题时的搜索引擎，尽量避免使用国产搜索引擎。 ***(请注意！这不是在歧视国产，而是根据笔者的使用经历得出的个人结论。仅供你在选择搜索引擎时作为参考意见)***

在开始之前你需要准备:

 1. 一份包含了 DoL 的zip压缩包。(一般为包含了 `Modloader`[^1] 的 DoL)

 2. 一部已安装包含高版本 <u>WebView</u> 的现代化浏览器的 Android 手机 **(是的，我知道你是因为系统 WebView 版本低又没办法更新，但又想玩 DoL 所以才来这的)**

 3. 安装一个好用的第三方文件管理器 ***(系统自带的一般仅有基础功能，可能无法满足需要，这里我推荐 [MT管理器](https://mt2.cn/download/)) ，接下来我有一步我会假设你也安装了MT管理器来举例***

 4. 一双灵巧的手和一个能举一反三并熟练使用浏览器进行搜索和翻译且懂得对手机文件进行基础操作的的大脑

### 开始

在 `/storage/emulated/0/` 下创建一个名为 `DoL` 的文件夹 ***(下文将这个文件夹称为 `$DoL`)*** 

你可以自己找别的地方创建，只要你自己能找到即可 ***(请注意，不要尝试在 `/` 添加和更改任何东西，你很有可能没有访问权限，即使有这也是个危险操作。但一般你会拥有往 `/storage/emulated/0/` 添加和更改的权限，但一样也要注意，因为其他应用可能也会往这里放文件)***

解压 DoL 的压缩包到 `$DoL`。解压方式、解压位置随意，只需保证文件会被正确释放并可以被浏览器访问到即可。

你应该会看到以下文件结构
```
$DoL
├── "Degrees of Lewdity VERSION.html.mod.html"
├── "Degrees of Lewdity VERSION.html.mod-polyfill.html"
├── "img"
└── "style.css"
```

在 `$DoL` 下创建一个 `.nomedia`[^2] 文件。创建后看起来应该是这样
```
$DoL
├── "Degrees of Lewdity VERSION.html.mod.html"
├── "Degrees of Lewdity VERSION.html.mod-polyfill.html"
├── "img"
├── ".nomedia"
└── "style.css"
```

:monocle_face: 在手机的设置中授予浏览器存储的访问权限[^3]

如果下面这个步骤失效，请继续尝试另外一个步骤

在浏览器地址栏输入 `file://$DoL/Degrees of Lewdity VERSION.html.mod.html`[^4] 应当就可以游玩了(祝你淫的愉快)

如果上一个步骤失效，你可以尝试在 `MT管理器` 中打开 `$DoL` 目录，然后长按 `Degrees of Lewdly VERSION.html.mod.html` 然后在弹出的窗口中点击 `打开方式` ，然后点击左下角的`类型` ，再点击 `全部` 然后找到你的现代化浏览器的图标，然后点它。应该就可以玩了

#### 这是个放在别的文件夹时要访问的网址的例子

我的游戏文件夹在这里

`/data/data/com.termux/files/usr/var/lib/proot-distro/installed-rootfs/archlinux/srv/http/Degrees of Lewdity/`[^5]

所以我就应该访问以下地址来玩游戏

`file:///data/data/com.termux/files/usr/var/lib/proot-distro/installed-rootfs/archlinux/srv/http/Degrees of Lewdity/Degrees of Lewdity VERSION.html.mod.html`

## 方法二(难搞但足够通用)

鸽了懒得写，反正没人催()

## 尾注

[^1]: Modloader 是 DoL 的模组加载器，也是现在使用汉化的前置条件。

[^2]: `.nomedia` 文件会告诉手机相册这里的图片不应被加入手机图库中，这个文件只需要在那里即可，它的内容是什么并不重要(你也不希望12000+的 DoL 资源图片挤满你的图库罢)

[^3]: 为浏览器授予存储的访问权限，可以让浏览器能够读写你手机的存储空间。这是必要的因为想让浏览器能够顺利读取 `$DoL` 文件夹，你需要给它这个权限。当然这也有利处，你可以直接在存档导出界面直接点击下载存档(这通常会使存档下载到 `/storage/emulated/0/download/` 当中)，你也可以直接导入存档而不用费劲的复制粘贴了。

[^4]: :monocle_face: `$DoL`必须为绝对路径，否则你将无法启动游戏

[^5]: 之所以这么长是因为我是用termux部署的本地服务端，然后访问本地服务端来玩游戏的，这里为了提供个对照直接把路径复制过来了，这个方法很繁琐，但是可以让你只要手机有在电脑上时也能直接访问手机来玩dol(手机已经成dol启动器了，加载游戏慢的要死，我都是电脑玩DoL了)
