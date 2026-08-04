乐富平台地址【Q-——333307——】乐富平台地址【 辋芷《888yx●vip》 】
乐富平台地址【Q-——333307——】乐富平台地址【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程

还在羡慕别人拥有独立博客？其实用 GitHub Pages 和 Hexo，半小时内就能搭建一个免费、稳定的个人网站。本教程手把手带你完成从环境配置到发布上线的全过程，无需服务器，零成本起步。

 为什么选择 Hexo + GitHub Pages？

- 完全免费：托管在 GitHub，不花一分钱
- 加载速度快：生成纯静态页面，国内访问表现优秀
- SEO 友好：文章收录效率高，适合沉淀技术笔记
- 高度定制：1000+ 主题自由切换，支持 Markdown 写作

 第一步：环境准备（3 分钟）

1. 安装 [Node.js](https://nodejs.org/)（选择 LTS 版本）
2. 安装 Git 并完成全局配置
3. 注册 GitHub 账号并创建仓库

 第二步：本地搭建 Hexo（5 分钟）

打开终端，逐行执行：

```bash
npm install hexo-cli -g    全局安装脚手架
hexo init my-blog          初始化项目
cd my-blog
npm install                安装依赖
hexo s                     本地预览
```

浏览器访问 `http://localhost:4000` 看到默认页面即成功。

 第三步：部署到 GitHub Pages（关键）

这里划重点：在 `_config.yml` 中修改部署信息：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

执行部署命令前，先安装自动部署插件：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo g && hexo d
```

等待命令行输出进度，访问 `你的用户名.github.io` 就能看到线上效果！

 第四步：文章发布与日常维护

写新文章只需两步：

```bash
hexo new post "我的第一篇文章"    创建草稿
 编辑 source/_posts/ 下的 md 文件后
hexo d   重新部署即更新站点
```

建议开启 GitHub 自动部署（Actions），以后只要 push 代码到仓库，网站自动更新，体验丝滑。

---

遇到问题怎么办？ 在评论区留言你的报错信息，或者私信回复“博客”获取我整理好的常见问题排查清单。如果你搭建成功，欢迎在评论区晒出你的博客链接，我会去参观学习！

收藏本文方便对照操作，关注我获取更多开发者效率工具干货。你的支持是我持续输出的最大动力！ 🚀

相关推荐：

https://github.com/sheppardrandall419/okbjfs/blob/main/2026%E7%A7%91%E6%8A%80%E7%83%AD%E6%A6%9C%EF%BC%9A%E4%B9%90%E5%AF%8C%E4%B8%BB%E7%AE%A1%E6%B5%8B%E9%80%9F_%E8%83%83%E8%AF%8D%E6%82%8D%E6%85%B0%E6%A1%A5OPQQY.md

<img src="https://i.postimg.cc/YSKHJZ5P/lefu-00006.png" />

相关推荐：

https://github.com/sheppardrandall419/okbjfs/commit/37fac4e877e18afedf731c341916df08ca641b1c

<img src="https://i.postimg.cc/XNH0VrMC/lefu-00016.png" />
相关推荐：

https://github.com/rhodesandrea462/zjvmux/blob/main/2026%E6%9D%83%E5%A8%81%E7%83%AD%E6%A6%9C%EF%BC%9A%E4%B9%90%E5%AF%8C%E4%B8%BB%E7%AE%A1%E4%BB%A3%E7%90%86_%E8%BE%97%E7%84%A6%E5%B4%96%E4%BB%93%E7%98%B8JJFMN.md

<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />
相关推荐：

https://github.com/rhodesandrea462/zjvmux/commit/21ee33e5736c87d773cfe4080c200c2bc591128f

<img src="https://i.postimg.cc/XNH0VrMC/lefu-00016.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
