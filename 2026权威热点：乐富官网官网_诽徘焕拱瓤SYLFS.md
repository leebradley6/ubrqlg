乐富官网官网【Q-——333307——】乐富官网官网【 辋芷《888yx●vip》 】
乐富官网官网【Q-——333307——】乐富官网官网【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程

作为一名开发者，拥有一个属于自己的技术博客，不仅是记录成长的方式，更是打造个人品牌、沉淀知识体系的关键一步。今天，我将手把手教你如何利用 GitHub Pages 和 Hexo，在半小时内搭建一个免费、高速、可定制的静态博客。

 为什么选择 GitHub Pages + Hexo？

- 零成本：GitHub Pages 提供免费静态托管，无需购买服务器。
- 极速访问：静态页面加载速度快，配合 CDN 全球加速。
- 版本管理：所有文章都是 Markdown 文件，天然支持 Git 版本控制。
- 高度定制：Hexo 拥有强大的主题生态，可轻松修改样式。

 搭建步骤详解

 1. 准备环境
首先，确保你的电脑安装了 Node.js 和 Git。没有安装的读者，请先前往官网下载对应版本。

 2. 安装 Hexo 并初始化
打开终端，输入以下命令：
```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
```
执行完毕后，本地博客骨架就搭建好了。

 3. 关联 GitHub 仓库
登录 GitHub，创建一个名为 `用户名.github.io` 的新仓库。然后在博客根目录下运行：
```bash
npm install hexo-deployer-git --save
```
修改 `_config.yml` 文件中的部署信息：
```
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
```

 4. 写文章并部署
创建新
```bash
hexo new "我的第一篇文章"
```
编辑 `source/_posts/` 下的 Markdown 文件，写好后执行：
```bash
hexo clean && hexo generate
hexo deploy
```
浏览器访问 `你的用户名.github.io`，就能看到你的博客上线了！

 进阶优化建议

- 绑定自定义域名：在仓库设置中添加 CNAME 文件，指向你的专属域名。
- 更换主题：Hexo 官网提供了数百款精美主题，一键切换。
- 添加评论系统：集成 Giscus 或 Valine，增加读者互动。

 常见问题排查

Q1：部署后页面空白？  
检查 `_config.yml` 中的 `url` 配置，确保与 GitHub Pages 地址一致。

Q2：图片不显示？  
将图片放在 `source/images/` 目录下，使用绝对路径引用。

Q3：如何备份博客源文件？  
将整个博客文件夹推送到另一个 Git 仓库，实现双保险。

---

搭建博客只是开始，坚持输出高质量的技术文章才是关键。如果你在搭建过程中遇到任何问题，欢迎在评论区留言，我们一起探讨解决。觉得这篇教程有用的话，请点赞、收藏并转发给身边需要的小伙伴，你的支持是我持续输出的最大动力！

相关推荐：

https://github.com/martinezjessica6229/eyvqwl/blob/main/%E7%A1%AC%E6%A0%B8%E5%85%A8%E9%98%B6%E6%94%BB%E7%95%A5%EF%BC%9A%E4%B9%90%E5%AF%8C_%E9%99%B6%E6%95%9B%E6%AD%89%E7%A9%86%E8%90%84AAAPD.md

<img src="https://i.postimg.cc/XJx6BJpR/lefu-00011.png" />

相关推荐：

https://github.com/martinezjessica6229/eyvqwl/commit/68cfea655ebfda1eae281f963a6d77681ca1d0b5

<img src="https://i.postimg.cc/XJx6BJpR/lefu-00011.png" />
相关推荐：

https://github.com/hoffmanandrew448/cbjrry/blob/main/2026%E7%AC%AC%E4%B8%80%E7%83%AD%E7%82%B9%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%A8%B1%E4%B9%90_%E6%80%9D%E7%A5%A8%E6%9E%97%E5%BA%95%E5%AD%9CEERJX.md

<img src="https://i.postimg.cc/YSKHJZ5P/lefu-00006.png" />
相关推荐：

https://github.com/hoffmanandrew448/cbjrry/commit/161d0215405d21a37bc601405ac2558f36accd41

<img src="https://i.postimg.cc/1XjxMj0W/lefu-00015.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
