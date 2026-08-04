乐富平台主管【Q-——333307——】乐富平台主管【 辋芷《888yx●vip》 】
乐富平台主管【Q-——333307——】乐富平台主管【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

还在羡慕别人炫酷的技术博客？其实搭建一个专属博客，比你想象中简单。利用 GitHub Pages 和 Hexo，无需购买服务器，完全免费，还能绑定自己的域名。今天手把手带你从零开始，十分钟上线你的第一个网站。

 为什么要用 GitHub Pages？

很多开发者首选它，核心优势很明确：免费托管、静态加速、版本管理天然集成。你写的 Markdown 文章，通过 Git 推送就能自动发布，完美适配技术人的工作流。而且百度对 GitHub Pages 的收录非常友好，利于 SEO 曝光。

 第一步：环境准备

在开始之前，你需要准备两样东西：

1. Node.js （建议 v18 以上版本）
2. Git （用于代码推送）

安装完成后，打开终端验证：
```bash
node -v
git --version
```
出现版本号即为成功。

 第二步：安装并初始化 Hexo

Hexo 是一个高速的静态博客框架，中文文档齐全，非常适合新手。

```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
```

初始化完成后，本地预览一下效果：
```bash
hexo s
```
浏览器访问 `http://localhost:4000` ，看到默认博客页面就说明你已经迈出了第一步。

 第三步：关联 GitHub 仓库

1. 在 GitHub 上新建一个仓库，命名必须为：`你的用户名.github.io`
2. 修改博客根目录下的 `_config.yml` 文件，找到 `deploy` 部分：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

然后执行：
```bash
npm install hexo-deployer-git --save
hexo g -d
```

等待几秒钟，访问 `https://你的用户名.github.io` ，你的博客就正式上线了！

 下一步该做什么？

完成部署后，你可以尝试：
- 更换主题：搜索 Hexo 主题，挑选喜欢的风格
- 发布将 Markdown 文件放入 `source/_posts`，运行 `hexo g` 即可生成
- 绑定域名：在仓库设置中添加 CNAME 文件，解析到你的域名

过程中遇到报错？别担心，这是每个开发者都会经历的。如果这篇文章帮到了你，请在下方评论区留言告诉我，或者顺手点个 Star 支持一下！你的每一次互动都是持续输出的动力。

想要看更多关于「自定义主题改造」或「SEO 优化技巧」的内容，记得关注我，关注不迷路，我们下期见！

相关推荐：

https://github.com/martinezjessica6229/eyvqwl/blob/main/%E7%A1%AC%E6%A0%B8%E5%85%A8%E9%98%B6%E6%94%BB%E7%95%A5%EF%BC%9A%E4%B9%90%E5%AF%8C_%E9%99%B6%E6%95%9B%E6%AD%89%E7%A9%86%E8%90%84AAAPD.md

<img src="https://i.postimg.cc/FKy4mGmf/lefu-00008.png" />

相关推荐：

https://github.com/martinezjessica6229/eyvqwl/commit/68cfea655ebfda1eae281f963a6d77681ca1d0b5

<img src="https://i.postimg.cc/tJTQ3j6x/lefu-00013.png" />
相关推荐：

https://github.com/hoffmanandrew448/cbjrry/blob/main/2026%E7%AC%AC%E4%B8%80%E7%83%AD%E7%82%B9%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%A8%B1%E4%B9%90_%E6%80%9D%E7%A5%A8%E6%9E%97%E5%BA%95%E5%AD%9CEERJX.md

<img src="https://i.postimg.cc/FKy4mGmf/lefu-00008.png" />
相关推荐：

https://github.com/hoffmanandrew448/cbjrry/commit/161d0215405d21a37bc601405ac2558f36accd41

<img src="https://i.postimg.cc/XqJSfb5x/lefu-00014.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
