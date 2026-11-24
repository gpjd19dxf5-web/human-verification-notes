# 人机验证工程研究

> 面向架构师、安全工程师和爬虫开发者的技术博客：图像挑战、人机验证、边缘风控、协议链路与安全评估。

## 在线站点

[打开 GitHub Pages 技术博客](https://gpjd19dxf5-web.github.io/human-verification-notes/)

## 理论基座：FunCaptcha 图像挑战与协议工程

这组三篇文章是本站的公共理论底座，后续顶象、Cloudflare 等平台专题都建立在相同的任务建模、工程评测和协议信任框架之上。

1. [问题建模、题型分类与数据工程](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/funcaptcha-image-modeling/)  
   任务边界、题型路由、数据切分和模型设计。

2. [训练、推理与评测](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/funcaptcha-recognition-engineering/)  
   训练流程、难例增强、置信度校准、推理编排和会话级评测。

3. [状态机、服务端校验与可观测性](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/funcaptcha-protocol-state-machine/)  
   挑战生命周期、短期凭证、重试语义、安全边界和可观测性。

理论专题总览：

[https://gpjd19dxf5-web.github.io/human-verification-notes/series/funcaptcha-theory/](https://gpjd19dxf5-web.github.io/human-verification-notes/series/funcaptcha-theory/)

## 平台专题：顶象人机验证

1. [系统架构与协议链路拆解](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/system-architecture-and-protocol/)
2. [风控 AI 与方案选型评估](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/risk-ai-and-solution-evaluation/)
3. [合规攻防评估实战](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/compliance-security-evaluation/)

## 边缘风控：Cloudflare 5s 盾

1. [Cloudflare 5s 盾原理：从挑战页到 cf_clearance 的风控链路](https://gpjd19dxf5-web.github.io/human-verification-notes/articles/cloudflare-5s-challenge/)

## 内容边界

本站公开内容以原理、架构、评估方法和工程框架为主，不发布第三方产品的未公开实现细节、私有协议、凭证伪造方法、完整核心算法或绕过脚本。相关研究与工具仅适用于自有系统、官方沙箱和书面授权环境。

## 仓库说明

- `index.md`：GitHub Pages 首页
- `articles/`：公开文章 Markdown 源文件
- `series/`：专题总览页
- `资产/images/`：文章配图
- `DEPLOY.md`：GitHub Pages 部署与维护说明

## 独立站

[访问 ocaptcha.com](https://ocaptcha.com)
