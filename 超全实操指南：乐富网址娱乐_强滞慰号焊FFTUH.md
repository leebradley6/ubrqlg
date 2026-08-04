乐富网址娱乐【Q-——333307——】乐富网址娱乐【 辋芷《888yx●vip》 】
乐富网址娱乐【Q-——333307——】乐富网址娱乐【 辋芷《888yx●vip》 】

 用GitHub Actions自动部署Hexo博客：从零到一完整指南

> 每次手动`hexo g`再`hexo d`，既繁琐又容易忘记？本文将带你用GitHub Actions实现推送即部署，彻底解放双手。

 为什么选择GitHub Actions？

GitHub Actions是GitHub原生提供的CI/CD服务，相比Travis CI等第三方工具，它拥有以下优势：

- 零成本：公共仓库完全免费
- 深度集成：与GitHub生态无缝衔接
- 配置简单：YAML文件即可完成自动化流程
- 生态丰富：官方和社区提供了大量现成Action

对于Hexo博客来说，利用Actions可以在你`git push`的那一刻自动完成`hexo g`构建和静态文件部署，让你的博客更新真正做到“一键发布”。

 前置准备

在开始之前，请确保你已完成以下操作：

1. 拥有一个GitHub账号并创建了博客仓库（例如`username.github.io`）
2. 本地已安装Node.js和Git
3. 已将Hexo博客项目初始化为Git仓库并推送到GitHub

 核心配置步骤

 第一步：生成部署密钥

我们需要为Actions提供推送权限。在本地终端执行：

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com" -f gh-pages-key
```

这会生成公钥和私钥。将私钥内容添加到GitHub仓库的`Settings → Secrets and variables → Actions`中，命名为`DEPLOY_KEY`。将公钥（`.pub`文件）添加到仓库的`Settings → Deploy keys`中，务必勾选“Allow write access”。

 第二步：编写工作流文件

在博客项目的`.github/workflows`目录下创建`deploy.yml`文件，内容如下：

```yaml
name: Deploy Hexo Blog

on:
  push:
    branches: [main]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4

      - name: Setup Node.js
        uses: actions/setup-node@v4
        with:
          node-version: '20'

      - name: Install dependencies
        run: npm ci

      - name: Build
        run: npm run build

      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v4
        with:
          deploy_key: ${{ secrets.DEPLOY_KEY }}
          publish_dir: ./public
```

这里使用了`peaceiris/actions-gh-pages`这个流行的Action，它会自动处理分支切换和文件推送。

 第三步：推送触发自动部署

将配置文件提交并推送：

```bash
git add .
git commit -m "Add GitHub Actions workflow"
git push origin main
```

推送后，进入仓库的`Actions`标签页，你会看到工作流正在运行。等待绿勾出现，你的博客就已经自动部署到`gh-pages`分支了。

 常见问题排查

- 构建失败：检查`package.json`中的`build`脚本是否存在，以及Node版本是否兼容
- 部署失败：确认`DEPLOY_KEY`设置正确，且公钥已添加到Deploy keys
- 页面404：检查GitHub Pages设置中Source是否选择了`gh-pages`分支

 进阶优化

- 添加缓存：在步骤中加入`actions/cache`缓存`node_modules`，可显著提速
- 多分支部署：可设置`on: push: branches: [main, dev]`实现测试分支预览
- 评论通知：通过`notify`步骤在构建完成后发送邮件或飞书通知

现在，每次你写完博客，只需要`git push`，剩下的全部交给GitHub Actions处理。快去体验自动化部署带来的爽快感吧！

---

互动引导：你在使用GitHub Actions部署过程中遇到过什么问题？欢迎在评论区留言讨论，或者分享你的自动化部署经验。如果觉得本文有用，别忘了一键三连支持下哦！

相关推荐：

https://github.com/richardsonhannah5/draixy/blob/main/%E6%95%B0%E5%AD%97%E6%96%87%E5%A8%B1%E5%8A%A8%E6%80%81%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%AE%98%E6%96%B9%E5%A8%B1%E4%B9%90_%E9%85%92%E7%BC%86%E7%BB%9F%E5%92%8F%E7%82%94XXDKR.md

<img src="https://i.postimg.cc/XNH0VrMC/lefu-00016.png" />

相关推荐：

https://github.com/richardsonhannah5/draixy/commit/8eb5af3bca27ae4c905e3ee4255d88c07e52f011

<img src="https://i.postimg.cc/XJx6BJpR/lefu-00011.png" />
相关推荐：

https://github.com/sheppardrandall419/okbjfs/blob/main/2026%E5%AE%98%E6%96%B9%E7%88%86%E7%82%B9%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%AE%98%E6%96%B9%E7%BD%91%E7%AB%99_%E8%B7%83%E9%9F%B6%E6%B8%8D%E8%A3%85%E5%B7%B1MSFGU.md

<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />
相关推荐：

https://github.com/sheppardrandall419/okbjfs/commit/ce1c23ece7bf701958d51502c6e9b974ec7b5238

<img src="https://i.postimg.cc/xTBDzB1n/lefu-00020.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
