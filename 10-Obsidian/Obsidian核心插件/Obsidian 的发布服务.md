---
uid: 20240429184002
title: Obsidian 发布服务
tags:
  - Obsidian
  - 核心插件
  - 发布
description: Obsidian 核心插件发布服务是为你的笔记提供的付费托管服务
author: OS
type: other
draft: false
editable: false
modified: 20240429232308
---

# Obsidian 发布服务

Obsidian 发布服务是为你的笔记提供的付费托管服务。

如果需要了解如何在 Obsidian 中发布笔记，请阅读 [这篇笔记](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E5%8F%91%E5%B8%83)。

### 隐私

即使使用 [发布](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E5%8F%91%E5%B8%83) 服务，你的隐私也是完全自主可控的。你可以自由选择需要发布的笔记，无论是几篇笔记还是整个库。那些你不想发布的笔记将永远不会为外界所知，Obsidian 也不会监测它们，它们将始终安全地保存在你的本地设备中。

### 备份

需要注意的是，发布服务并不是用于备份笔记的。如需备份笔记，请使用那些符合你喜好且稳定的备份方法。Obsidian 的发布服务将更侧重于功能性、易用性以及网站的稳定性。

### 示例

如果你还没见过使用发布服务发布出来的网站，那么可以看看这个：[https://publish.obsidian.md/help](https://publish.obsidian.md/help) （英文）。

### 服务内容

Obsidian 发布服务作为内置功能可以让你选用库中的笔记来直接搭建一个自己的网站。

你可以对这个网站进行个性化设置，比如选择网站的配色方案，切换可见行宽。

一些网站组件可以在 [发布插件](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E5%8F%91%E5%B8%83) 中启用或关闭。对这些选项的修改需要清除缓存后才会体现在发布的网站上，一般 5 分钟之内可以完成。

##### 导航栏

开启这个组件后会在网站左边显示一个导航栏，导航栏将显示所有已发布的笔记以及包含它们的文件夹。当前正在访问的页面会在导航栏中高亮显示。

##### 搜索栏

在导航栏开启的前提下你可以开启搜索栏。搜索栏允许访问者搜索页面标题及小标题。目前搜索栏不支持全文内容检索。

##### 局部关系图

开启后将展示每个页面的局部关系图。这与 Obsidian 中的 [关系图谱](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E5%85%B3%E7%B3%BB%E5%9B%BE%E8%B0%B1) 使用的是同样的引擎。

##### 大纲

开启后将展示当前页面的大纲。大纲由页面中的小标题组成，这和 Obsidian 中的 [大纲](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E5%A4%A7%E7%BA%B2) 是一样的。

大纲会以高亮形式提示访问者当前正在浏览页面的哪一部分。访问者可以通过点击大纲来在页面上的内容间快速跳转。

##### 反向链接

开启后，每页末尾将显示一个名为 `Linked to this page` 的部分，这个部分中展示了当前页面的反向链接。如果当前页面没有反向链接，此部分将不会显示。

##### 标签

当访问者点击页面上的标签时，网站会弹出一个窗口，其中列出了所有包含该标签的页面。

##### 悬停预览

开启这个组件后，访问者鼠标悬停在页面上的链接时，会看到一个弹出窗口，窗口中显示了链接的内容。这和 [页面预览](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E9%A1%B5%E9%9D%A2%E9%A2%84%E8%A7%88) 一样。

##### 自定义 CSS

如果想进一步设置网站的主题，你可以上传自定义 CSS 文件。需要注意的是，自定义 CSS 文件需要命名为 `obsidian.css` 或 `publish.css`，并且放置在网站所在的库的根目录下，这样才能上传并使用。

这里建议你使用 `publish.css` 来命名网站的主题文件，这样 `obsidian.css` 能用于你本地的主题文件，从而实现本地主题和网站主题的区分。

##### Favicon

如果想修改网站图标，你可以上传 `png` 格式的图标图片，并将其以 `favicon-32.png` 或 `favicon-32x32.png` 的形式命名。

你也可以通过上传文件 `favicon.ico` 来修改网站图标。

这些图标文件可以存放在库中的任何位置。当前（2020 年）推荐的图标大小为 `32×32`，`128x128`，`152×152`，`167x167`，`180x180`，`192x192`，以及 `196x196`。

##### 自定义 JS

如果你希望执行自己编写的 JavaScript 代码以提升访客的浏览体验，或是为自己的网站增加一些功能（如 Discus!、Discourese 等），你可以创建一个 `publish.js` 文件并将其放至于库的根目录后将其上传。需要注意的是，这些脚本仅对于你网站的访客生效。

##### 禁止搜索引擎索引

这个选项会为你所有页面添加 meta noindex 设置，从而使得 Google 这样的搜索引擎无法索引你的网站。如果你的网站设置了密码保护，搜索引擎无论如何也无法索引你的网站。

##### Google Analytics

如果你希望为你的网站启用 Google Analytics，请先确保当地法律法规允许你这么做。然后，你需要将诸如 `UA-XXXXX-Y` 的追踪代码填入相应的文本框中，随后你的网站就会被自动追踪访问情况。注意，Google Analytics 仅对从你自定义域名来的流量有效。

测试 Google Analytics 的时候，请先关闭浏览器上的去广告扩展（比如 uBlock Origin 等），这些扩展会影响 Google Analytics 的代码运行。

另外，发布服务目前还不能直接与 Google Tag Manage 兼容——如果你想使用 Google Tag Manage 而不是 Google Analytics，你可以使用自定义 javascript 设置它。

### 自定义域名

你可以为你的网站设置自定义域名。目前，我们还没有办法为你提供 SSL 证书，因此你需要自行寻找启用 SSL 的服务器，或者在 CloudFlare 上设置您的网站，他们免费提供 SSL 证书服务。

你也可以将 Obsidian 发布的内容作为你自己网站的子 URL，比如 `https://my-site.com/my-notes/`。要实现这一点，你必须要有自己的服务器，并将所有请求代理到我们的服务器上 `https://publish.obsidian.md/`。

#### CloudFlare 设置

设置自定义域名或子域名的最简单方法就是使用 [CloudFlare](https://cloudflare.com/)，并让 CloudFlare 管理你的域名。这样你就可以免费向你的网站添加 SSL，同时确保你的网站在世界任何地方都能被快速访问。

你只需要添加一个 CNAME 记录到你的域或子域，将值设置为 `publish-main.obsidian.md`。然后，转到 SSL/TLS 配置，并将 SSL/TLS 加密模式设置为 `Full`。这将自动配置 SSL/TLS 证书。

一旦完成了 CloudFlare 的配置，你就可以在 Obsidian 中设置你的网站选项，并将 URL 设置为你的域或子域，从而允许我们的服务器将域与你的网站相关联。

#### 代理/重定向设置

如果你希望托管自己的 web 服务器并设置自己的 SSL 加密，则可以选择此选项。如果你已经托管一个网站在你的域或子域，你也可以通过使用这个选项让你的网站以特定的 URL 路径加载你通过 Obsidian 发布的网站。

要做到这点，只需简单地将所有该 URL 路径下的请求代理到 `https://publish.obsidian.md/serve?url=my-domain.com/my-subpath/...`，并在 Obsidian 的网站设置中配置相同的 URL 路径。

比如，在 NGINX 中，你可以如下设置：

```nginx
location /my-notes {
	proxy_pass https://publish.obsidian.md/serve?url=my-domain.com/my-notes/;
	proxy_ssl_server_name on;
}
```

在 Apache 的 `.htaccess`，你可以如下设置：

（注意：mod_rewrite 必须开启，并且你需要配置 [SSLProxyEngine](https://stackoverflow.com/questions/40938148/reverse-proxy-for-external-url-apache))

```htaccess
RewriteEngine  on
RewriteRule    "^my-notes/(.*)$"  "https://publish.obsidian.md/serve?url=my-domain.com/my-notes/$1"  [L,P]
```

如果你使用 Netlify，你可以如下设置：

```
[[redirects]]
  from = "https://my-domain.com/my-notes/*"
  to = "https://publish.obsidian.md/serve?url=my-domain.com/my-notes/:splat"
  status = 200
  force = true
```

#### 自定义域名设置之后的问题

你设置了自定义域名，但如果你以前从 `https://publish.obsidian.md/slug` 访问过你的网站的话，你可能需要清除浏览器缓存（比如字体、图片或访问密码等）使其能正常访问。这是由于现代浏览器强加的跨域安全限制导致的。好消息是，如果你只让你的访问者使用自定义域名，他们就永远不会遇到这个问题。

### 未来计划

发布服务仍处于早期阶段，以下是我们计划添加的一些功能：

- 完整的自定义域名支持（提供 SSL 证书）
- 全文检索
- 更多内置主题

如果你对发布服务有任何建议或意见，请通过在 [论坛](https://forum.obsidian.md/) 发帖让我们知道。

### 价格

关于发布服务的价格，请看 [我们的价格说明](https://obsidian.md/pricing)。

### 技术细节

Obsidian 发布服务使用 CloudFlare 作为 CDN（内容分发网络）来在全球范围内分发你的网站，以实现网站的更快访问。其原理是在 200 多个数据中心缓存你网站的文件副本，从而保证你的网站在任何地方都有较快的加载速度。

但这意味着当你修改网站设置、发布或取消发布内容时，访问者可能无法立即看到最新版本的网站。目前，我们将网站缓存设置为一个小时，超过一个小时后就必须重新验证，从而确保所访问版本是最新的。

如果你刚刚发布了一些内容，但是看到的仍然是网站的旧版本，你可以尝试按住重新加载按钮并在下拉菜单中选择 `hard reload` 来执行 `hard refresh`。如果这个方法不行，你还可以尝试清除浏览器缓存或使用开发者工具禁用缓存。

---

### 相关信息

你可以阅读 [发布](https://publish.obsidian.md/help-zh/%E6%8F%92%E4%BB%B6/%E5%8F%91%E5%B8%83) 来获取更多关于如何发布笔记的信息。