乐富注册代理【Q-——333307——】乐富注册代理【 辋芷《888yx●vip》 】
乐富注册代理【Q-——333307——】乐富注册代理【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025最新版）

还在羡慕别人拥有独立博客？其实你离技术博主只差30分钟。本文基于最新版Hexo 7.x，手把手教你用GitHub Pages免费部署个人网站，无需服务器，无需域名，全程零成本。

 为什么选择GitHub Pages + Hexo？
- 完全免费：静态托管无限流量，全球CDN加速
- 高度定制：支持自定义主题，Markdown写作，SEO友好
- 版本管理：借助Git天然优势，文章更新可追溯

 第一步：环境准备（3分钟）
在开始前，先确保本地环境满足以下条件：

1. 安装Git（Windows需配置环境变量）
2. 安装Node.js（建议v18以上版本，自带npm）
3. 注册GitHub账号并配置SSH密钥（`ssh-keygen -t ed25519` 生成）

遇到环境配置问题？ 在评论区留言，我看到会尽快回复。

 第二步：快速搭建Hexo框架（5分钟）
打开终端执行以下命令（Mac/Linux使用terminal，Windows使用Git Bash）：

```bash
npm install -g hexo-cli   全局安装Hexo脚手架
hexo init my-blog         初始化博客项目
cd my-blog                进入项目目录
npm install               安装依赖包
hexo server               本地预览 http://localhost:4000
```

看到默认页面即表示成功。此时修改`_config.yml`文件中的`title`、`author`等基础信息，刷新浏览器即可看到你的专属站名。

 第三步：部署到GitHub（10分钟）
1. 在GitHub新建仓库，命名格式必须为 `用户名.github.io`
2. 安装自动部署插件：
```bash
npm install hexo-deployer-git --save
```
3. 修改`_config.yml`部署部分：
```yaml
deploy:
  type: git
  repo: git@github.com:用户名/用户名.github.io.git
  branch: main
```
4. 执行部署命令：
```bash
hexo clean && hexo generate
hexo deploy
```

 第四步：绑定自定义域名（可选）
如需个性域名，在仓库Settings的Pages设置中填写域名，并在域名服务商添加CNAME记录指向`用户名.github.io`。然后在`source`目录新建`CNAME`文件，内容为你的域名。

 进阶优化建议
- 安装 `hexo-admin` 实现网页端写作
- 配置 `hexo-generator-sitemap` 生成站点地图
- 使用 `hexo-abbrlink` 生成固定文章链接（利于SEO）

完整源码与新手指南已打包，关注并私信回复“博客教程”，我会第一时间自动发送给你。有任何安装问题，欢迎在评论区交流经验，我看到都会互动解答。

相关推荐：

https://github.com/larsenpaul061/lcndhr/blob/main/2026%E7%A7%91%E6%8A%80%E6%89%8B%E5%86%8C%EF%BC%9A%E4%B9%90%E5%AF%8C%E7%BD%91%E5%9D%80_%E5%9F%8E%E8%B4%A8%E5%93%A6%E5%88%83%E7%89%A2NVVYG.md

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />

相关推荐：

https://github.com/larsenpaul061/lcndhr/commit/cb3a98dd50ba520d900163465f9bb6212ea4cb82

<img src="https://i.postimg.cc/XNH0VrMC/lefu-00016.png" />
相关推荐：

https://github.com/leebradley6/ubrqlg/blob/main/2026%E7%A7%91%E6%8A%80%E5%A4%8D%E7%9B%98%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%9C%B0%E5%9D%80_%E9%98%91%E8%B4%AD%E5%90%95%E6%8D%85%E7%93%9CVIIRE.md

<img src="https://i.postimg.cc/tJTQ3j6x/lefu-00013.png" />
相关推荐：

https://github.com/leebradley6/ubrqlg/commit/350a0f70d2fe35534b9de76165019e4a1b514bc8

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
