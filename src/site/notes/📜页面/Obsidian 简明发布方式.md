---
{"dg-publish":true,"permalink":"/📜页面/Obsidian 简明发布方式/","noteIcon":"1","created":"2023-05-12T14:30:04.573+08:00","updated":""}
---


##### 前言
使用 Obsidian 写好笔记后，有的时候想把自己的笔记分享给朋友，有的时候想把笔记发布到网络上，作为个人博客或者数字花园。而 Obsidian 是基于本地存储的 markdown 笔记，这就意味着无法直接生成网页链接发给朋友，要么使用 Obsidian 的官方发布服务，要么通过部署个人网站将 markdown 文件生成网页进行发布。现有介绍较多的一些发布方案已经足够简单，但是往往需要电脑端，需要 git，需要简单的代码等等，门槛还是略高。因此本文介绍一种更为简单可用的 Obsidian 发布方式。
##### 概述
本文介绍一种简明的 Obsidian 发布方式，不需要电脑，不需要会代码，不需要特殊网络，不需要使用其他软件，仅仅需要在手机上点点点即可完成。
这些通过使用插件 [Obsidian Digital Garden](https://github.com/oleeskild/Obsidian-Digital-Garden) 来实现，笔记文件托管在 [GitHub](https://github.com) 上，通过 [Netlify App](https://app.netlify.com/) 部署发布，不需要任何费用。
不知道为什么介绍使用这个插件的文章很少，而我在配置的时候也踩了两个坑，导致一开始并没用发布成功。
现在就一步一步的跟着做吧。如果你也想拥有自己的个人博客或者说数字花园。

##### 第一步 部署网站
是的没错，我们现在就开始部署网站了😊。
1. 点击 [Deploy to Netlify](https://app.netlify.com/start/deploy?repository=https://github.com/oleeskild/digitalgarden)

2. 点击网页中 "Connect to GitHub" 按钮。如果要登录的话就注册一个 Github 账号登录。
	![Screenshot_2023-05-12-15-32-58-814_com.lemurbrowser.exts.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/Screenshot_2023-05-12-15-32-58-814_com.lemurbrowser.exts.jpg)
3. 在 "Repository name" 框中输入一个存放笔记的 Github 仓库名称。或者直接使用默认的 "digitalgarden"。
	![Screenshot_2023-05-12-15-34-09-601_com.lemurbrowser.exts.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/Screenshot_2023-05-12-15-34-09-601_com.lemurbrowser.exts.jpg)
4. 点击 "Save & Deploy" 按钮。
5. 出现下面这个界面就说明部署好了。
	![Screenshot_2023-05-12-16-18-40-675_com.lemurbrowser.exts.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/Screenshot_2023-05-12-16-18-40-675_com.lemurbrowser.exts.jpg)
6. 上图中 "Permalink" 这个链接点进去就是你的网站啦。当然现在还没有内容。
	![Screenshot_2023-05-12-16-19-44-251_com.lemurbrowser.exts.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/Screenshot_2023-05-12-16-19-44-251_com.lemurbrowser.exts.jpg)
##### 第二步 安装插件
在 Obsidian 插件市场中搜索下载安装即可。
##### 第三步设置插件
1. 获取 Github 密钥。点击 [access token](https://github.com/settings/tokens/new?scopes=repo)，noto 输入框随便填一下英文名称，expiration 选 no expiration。往下滑点击 "Generate token"按钮并复制密钥待用。
	![Screenshot_2023-05-12-17-32-07-343_com.lemurbrowser.exts.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/Screenshot_2023-05-12-17-32-07-343_com.lemurbrowser.exts.jpg)
2. 打开插件 "Digital Garden" 的设置页面。将之前设置的"Repository name"填入 repo name，username 填入 Github 的用户名，token 填入上面一步获得的密钥。URL 填入之前的"Permalink"。
	![IMG_20230512_174133.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/IMG_20230512_174133.jpg)
3. 继续往下滑动设置页面，将下图中的选项关掉。
	![Screenshot_2023-05-12-17-40-23-752_md.obsidian-edit.jpg](/img/user/%F0%9F%93%A6%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/Screenshot_2023-05-12-17-40-23-752_md.obsidian-edit.jpg)

##### 第四步发布笔记
好啦现在就可以发布笔记到你的网站上啦。
打开笔记页面，搜索并打开命令 "Digital Garden: Quick Publish And Share Note"，笔记就发布好啦，并且自动将页面链接复制到剪贴板上，过一会在浏览器打开链接就可以看到发布好的页面🚀。
