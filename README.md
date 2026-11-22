# 人机验证工程研究 · GitHub Pages

这是一个可直接部署到 GitHub Pages 的 Jekyll 站点骨架。公开文章只保留原理、架构、评估框架和思路，不包含核心实现、私有协议或绕过工具。

## 目录

```text
.
├── _config.yml
├── index.md
├── about.md
├── 404.md
├── robots.txt
├── _layouts/
│   └── article.html
├── _includes/
│   └── advanced-cta.html
├── assets/
│   └── main.scss
└── articles/
    ├── 01-system-architecture-and-protocol.md
    ├── 02-risk-ai-and-solution-evaluation.md
    └── 03-compliance-security-evaluation.md
```

## 发布前替换

打开 `_config.yml`，替换：

```yaml
url: "https://gpjd19dxf5-web.github.io"
baseurl: "/human-verification-notes"
author: "black A"
advanced_url: "https://ocaptcha.com"
```

打开 `about.md`，替换作者和独立站链接。

## 部署到 GitHub Pages

1. 新建一个公开仓库，例如 `human-verification-notes`。
2. 将本目录全部文件上传到仓库根目录。
3. 进入仓库 `Settings` → `Pages`。
4. `Build and deployment` 选择 `Deploy from a branch`。
5. Branch 选择 `main`，目录选择 `/ (root)`。
6. 保存后等待 GitHub Actions/Pages 构建完成。
7. 访问 `https://gpjd19dxf5-web.github.io/human-verification-notes/`。

## 本地预览

如果本机有 Ruby 和 Bundler：

```bash
bundle install
bundle exec jekyll serve
```

然后访问终端提示的本地地址。

## 内容策略

公开仓库只放：

- 系统架构；
- 抽象协议状态机；
- 风控模型概念；
- 评估方法和指标；
- 风险与防御清单；
- 独立站进阶入口。

不要把以下内容提交到公开仓库：

- 第三方产品未公开的接口、参数和加密实现；
- 可工作的绕过、伪造、重放或批量攻击脚本；
- 真实 token、Cookie、密钥、用户数据；
- 完整核心算法、模型权重和私有数据；
- 未授权的测试记录。

GitHub Pages 是静态公开站点。任何被提交到仓库根目录或文章目录的文件，即使没有站内链接，也可能被直接访问、被搜索引擎发现，或从 Git 历史中恢复。真正的进阶内容应放在独立站或私有仓库，不要只靠“不放出链接”来保护。

## SEO 建议

- 每篇文章使用独立、描述性的英文 URL；
- 保留独立标题和 `description`；
- 通过首页和三篇文章互相内链；
- 部署后在 Google Search Console 和 Bing Webmaster Tools 提交 `sitemap.xml`；
- 保持 `robots.txt` 允许抓取；
- 不要在页面中堆砌关键词，围绕“人机验证架构、挑战协议、风控模型、合规评估”持续写有实质内容的长文。
