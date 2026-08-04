乐富主管客服【Q-——333307——】乐富主管客服【 辋芷《888yx●vip》 】
乐富主管客服【Q-——333307——】乐富主管客服【 辋芷《888yx●vip》 】

 从0到1搭建个人技术博客：GitHub Pages + Hexo 完整指南

> 还在为写技术文章无处安放而烦恼？手把手教你用 GitHub Pages 免费搭建个人技术博客，支持自定义域名、SEO优化，一次配置永久使用。文末附赠SEO关键词布局清单。

 为什么选择 GitHub Pages 搭建博客？

作为技术人，GitHub Pages 拥有三大不可替代的优势：
- 完全免费：无需购买服务器，GitHub 免费提供静态托管
- 版本管理：所有文章通过 Git 管理，天然具备备份和协作能力
- SEO友好：静态页面加载速度快，百度收录率远高于动态博客

 三步完成博客搭建

 第一步：创建 GitHub 仓库
1. 新建仓库，命名为 `你的用户名.github.io`
2. 勾选 “Add a README file” 初始化仓库
3. 记住仓库地址，后续部署需要用到

 第二步：本地安装 Hexo 框架
```bash
npm install hexo-cli -g    全局安装Hexo
hexo init my-blog          初始化博客目录
cd my-blog                 进入博客目录
npm install                安装依赖包
```

> 小提示：建议使用 Node.js 14+ 版本，避免依赖冲突。

 第三步：部署到 GitHub
修改根目录 `_config.yml` 中的 deploy 配置：
```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```
然后执行：
```bash
hexo clean && hexo generate && hexo deploy
```

 提升文章收录的5个SEO技巧

根据百度搜索引擎优化指南，技术博客需要注意：
1. URL结构：在 `_config.yml` 中设置 `permalink: :year/:month/:title/`
2. 标题优化：每个页面确保包含核心关键词（如“GitHub Pages教程”）
3. 内部链接：文章之间互相推荐，增加爬虫抓取路径
4. 代码高亮：开启 `highlight` 功能，增强代码可读性
5. 更新频率：每周至少发布1篇，保持站点活跃度

 进阶优化建议

若想进一步提升访问体验，可以：
- 使用 [hexo-generator-sitemap](https://github.com/hexojs/hexo-generator-sitemap) 插件生成站点地图
- 在 Google Search Console 提交验证，加速收录
- 参考相关主题配置，比如 [Next主题文档](https://theme-next.js.org/)

---

你的技术文章现在有了归宿，立即动手搭建属于你的技术博客吧。如果遇到问题，欢迎在评论区留言交流，我将在24小时内回复。别忘了把这份指南分享给同样需要搭建博客的朋友，让知识流动起来。

相关推荐：

https://github.com/jarvisdanielle312/mphvpi/blob/main/2026%E5%AE%98%E6%96%B9%E5%A4%8D%E7%9B%98%EF%BC%9A%E4%B9%90%E5%AF%8C%E7%BD%91%E5%9D%80%E4%B8%BB%E7%AE%A1_%E8%AF%9C%E5%9F%A0%E6%BD%9C%E9%97%BB%E6%AE%96QJXRG.md

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />

相关推荐：

https://github.com/jarvisdanielle312/mphvpi/commit/1c0bed8a749e26577d6031a5f5af60a6a89ce358

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />
相关推荐：

https://github.com/leebradley6/ubrqlg/blob/main/%E6%B2%89%E9%86%89%E6%96%87%E5%BF%83%E5%AF%BB%E6%A2%A6%EF%BC%9A%E4%B9%90%E5%AF%8C%E4%B8%BB%E7%AE%A1%E5%B9%B3%E5%8F%B0_%E5%87%89%E8%B6%9F%E6%8B%BC%E4%B8%88%E9%9B%8DNUGUW.md

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />
相关推荐：

https://github.com/leebradley6/ubrqlg/commit/100102b91bd194dd059d254f5693b0987e06c3fb

<img src="https://i.postimg.cc/XJx6BJpR/lefu-00011.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
