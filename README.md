# 在安卓手机上运行以zip格式进行分发的《Degrees of Lewdly》

## 开始之前

请注意，本教程只负责教你如何安装和打开<u>Degrees of Lewdly**(在下文里简称 `DoL`)**</u>，汉化和美化的安装并不包括在哪。

当你看到 :monocle_face: 时如果你对当前步骤，感到不解或者不知道怎么做的时候请去使用浏览器搜索，因为这只是一篇简易教程不会开太长篇幅讲和目标无太大关联的东西(这里我有一个个人建议，使用bing或其他国外搜索引擎作为你搜索问题时的搜索引擎，避免使用国产搜索引擎。<u>**注意！这不是歧视国产，而是根据笔者的使用经历得出的个人结论。仅供你在选择搜索引擎时作为参考意见**</u>)

但关于汉化安装你可以前往 [Degrees-of-Lewdity-Chinese-Localization](https://github.com/Eltirosto/Degrees-of-Lewdity-Chinese-Localization) 阅读该仓库的 README，该仓库也是汉化的发布仓库，你可以在该仓库里获取最新版的汉化 Mod。
如有任何关于汉化问题问题，请先熟读并背诵 README 全文然后去看看 Issue 里有没有相同问题再发问。
发问前请阅读 [提问的智慧](https://lug.ustc.edu.cn/wiki/doc/smart-questions) 以提高你的问题被注意和回答的可能性，请记住，礼貌永远能让人更乐意耐心解答你的问题，礼多人不怪。

你可以在 [Releases](https://github.com/Eltirosto/Degrees-of-Lewdity-Chinese-Localization/releases) 获取DoL的 Modloader 以及图片资源包和汉化 Mod

在此之前你需要准备:

 1. 一份包含了 DoL 的zip压缩包。(一般为包含了 Modloader 的 DoL)
 2. 一部已安装包含高版本 <u>WebView</u> 的现代化浏览器的 Android 手机(是的，我知道你是因为系统 WebView 版本低又没办法更新，但又想玩 DoL 所以才来这的)
 3. 安装一个好用的第三方文件管理器(系统自带的一般仅有基础功能，可能无法满足需要，这里我推荐 [MT管理器](https://mt2.cn/download/))(可选)
 3. 一双灵巧的手，和一个能举一反三并熟练使用浏览器进行搜索和翻译并懂得对手机文件进行基础操作的的大脑

## 开始

在 `/storage/emulated/0/` 下创建一个名为 `DoL` 的文件夹，你可以自己找别的地方创建只要你自己能找到即可(下文将这个文件夹称为 `$DoL`)

解压 DoL 的压缩包到 `$DoL`。解压方式、解压位置随意，只需保证文件会被正确释放并可以被浏览器访问到即可。

你应该会看到以下文件结构
```
$DoL
├── "Degrees of Lewdity VERSION.html.mod.html"
├── "Degrees of Lewdity VERSION.html.mod-polyfill.html"
├── "img"
└── "style.css"
```

在 `$DoL` 下创建一个 `.nomedia`[^1] 文件。创建后看起来应该是这样
```
$DoL
├── "Degrees of Lewdity VERSION.html.mod.html"
├── "Degrees of Lewdity VERSION.html.mod-polyfill.html"
├── "img"
├── ".nomedia"
└── "style.css"
```

:monocle_face: 在手机的设置中授予浏览器存储的访问权限[^2]

在浏览器地址栏输入"file://$DoL/Degrees of Lewdity VERSION.html.mod.html"应当就可以游玩了，你如果已经完成了一切而且是完全按照我的指导一步步来的那么你现在点击这个链接[file:///storage/emulated/0/DoL/Degrees of Lewdity VERSION.html.mod.html](file:///storage/emulated/0/DoL/Degrees of Lewdity VERSION.html.mod.html)就可以直接开始游戏了(祝你淫的愉快)

---

我的游戏文件夹在

`/data/data/com.termux/files/usr/var/lib/proot-distro/installed-rootfs/archlinux/srv/http/Degrees of Lewdity/`[^3]

所以我就应该访问

`file:///data/data/com.termux/files/usr/var/lib/proot-distro/installed-rootfs/archlinux/srv/http/Degrees of Lewdity/Degrees of Lewdity VERSION.html.mod.html`

来玩游戏

---

## 尾注

[^1]: `.nomedia` 文件会告诉手机相册这里的图片不应被加入手机图库中，这个文件只需要在那里即可，它的内容是什么并不重要(你也不希望12000+的 DoL 资源图片挤满你的图库罢)

[^2]: 为浏览器授予存储的访问权限，可以让浏览器能够读写你手机的存储空间。这是必要的因为想让浏览器能够顺利读取 `$DoL` 文件夹，你需要给它这个权限。当然这也有利处，你可以直接在存档导出界面直接点击下载存档(这通常会使存档下载到 `/storage/emulated/0/download/` 当中)，你也可以直接导入存档而不用费劲的复制粘贴了。

[^3]: 之所以这么长是因为我是用termux部署的本地服务端，然后访问本地服务端来玩游戏的，这里为了提供个对照直接把路径复制过来了，这个方法很繁琐，但是可以让你只要手机有在电脑上时也能直接访问手机来玩dol(手机已经成dol启动器了，加载游戏慢的要死，我都是电脑玩DoL了)
