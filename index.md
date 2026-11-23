---
layout: page
title: 人机验证工程研究
permalink: /
---

> 从系统架构、协议链路到边缘风控：写给架构师、安全工程师和爬虫开发者的技术研究笔记。

## 这个系列解决什么问题

人机验证经常被简化为“识别验证码”。但在真实系统里，题目只是最外层。真正决定安全与体验的，是前端信任边界、挑战状态机、服务端校验、风险模型和可观测性共同组成的链路。

本系列不披露第三方产品未公开的实现细节，也不提供绕过、伪造凭证或攻击代码。我们更关注：

- 系统如何分层，信任边界在哪里；
- 一次挑战如何从下发走到服务端裁决；
- 风控 AI 如何从信号走到策略；
- 如何评估误接受、误拒绝、延迟和隐私成本；
- 如何在授权环境中做可复现的安全评估。

## 研究文章

<div class="article-grid">
  <a class="article-card" href="{{ '/articles/system-architecture-and-protocol/' | relative_url }}">
    <span class="article-index">01</span>
    <h2>系统架构与协议链路拆解</h2>
    <p>拆解客户端、挑战服务、风险决策和业务服务端之间的信任边界。</p>
    <span class="article-link">开始阅读 →</span>
  </a>

  <a class="article-card" href="{{ '/articles/risk-ai-and-solution-evaluation/' | relative_url }}">
    <span class="article-index">02</span>
    <h2>风控 AI 与方案选型评估</h2>
    <p>理解风险信号、模型校准、漂移监控和方案选型评分卡。</p>
    <span class="article-link">开始阅读 →</span>
  </a>

  <a class="article-card" href="{{ '/articles/compliance-security-evaluation/' | relative_url }}">
    <span class="article-index">03</span>
    <h2>合规攻防评估实战</h2>
    <p>用授权测试、威胁建模和指标体系替代不可持续的“完整逆向”。</p>
    <span class="article-link">开始阅读 →</span>
  </a>

  <a class="article-card" href="{{ '/articles/cloudflare-5s-challenge/' | relative_url }}">
    <span class="article-index">04</span>
    <h2>Cloudflare 5s 盾原理</h2>
    <p>拆解挑战页、cf_clearance、TLS 指纹与多层风控的真实链路。</p>
    <span class="article-link">开始阅读 →</span>
  </a>
</div>

## 适合谁阅读

- 正在设计登录、注册、支付、营销和内容安全链路的架构师；
- 需要评估第三方人机验证组件质量的后端与平台工程师；
- 研究风控模型、误伤率和可观测性的算法工程师；
- 需要理解 Cloudflare 边缘风控、TLS 指纹与合规访问边界的爬虫开发者；
- 在授权范围内开展安全评估的红队与安全工程团队。

## 进阶内容

公开文章保留原理、思路和框架；完整的评估模板、工程实现细节和工具链会整理在独立站。你可以从每篇文章末尾的进阶入口继续阅读。

> 研究边界：对任何第三方人机验证系统进行逆向、自动化测试或压力测试，都应事先取得明确授权。本站内容适用于自有系统、官方沙箱、测试账号和书面授权范围内的安全评估。
