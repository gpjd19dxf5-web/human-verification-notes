---
layout: page
title: "理论基座：FunCaptcha 图像挑战与协议工程"
description: "从视觉任务建模、训练评测到协议状态机，建立人机验证与图像挑战研究的理论基础。"
permalink: /series/funcaptcha-theory/
---

> 这是一个理论专题：不追求某一次“通过”，而是解释图像挑战如何被建模、训练、评测，并接入一条可校验的协议链路。

## 为什么把这组文章作为理论基座

后续的顶象人机验证、Cloudflare 5s 盾和其他风控系统，虽然产品形态不同，但都可以落回三个基础问题：

1. **视觉任务如何定义？** 是分类、检测、OCR，还是多步交互？
2. **模型如何被工程化？** 数据切分、置信度校准、推理编排和评测指标如何闭环？
3. **协议如何建立信任？** 客户端提交证据，服务端如何校验、绑定和审计？

这三篇文章构成后续平台专题的共同理论底座。

## 三篇理论文章

<div class="article-grid">
  <a class="article-card" href="{{ '/articles/funcaptcha-image-modeling/' | relative_url }}">
    <span class="article-index">01</span>
    <h2>问题建模、题型分类与数据工程</h2>
    <p>先定义任务和会话目标，再设计题型路由、数据切分和模型结构。</p>
    <span class="article-link">开始阅读 →</span>
  </a>

  <a class="article-card" href="{{ '/articles/funcaptcha-recognition-engineering/' | relative_url }}">
    <span class="article-index">02</span>
    <h2>训练、推理与评测</h2>
    <p>从轻量基线、难例增强、置信度校准到推理编排和会话级评测。</p>
    <span class="article-link">开始阅读 →</span>
  </a>

  <a class="article-card" href="{{ '/articles/funcaptcha-protocol-state-machine/' | relative_url }}">
    <span class="article-index">03</span>
    <h2>状态机、服务端校验与可观测性</h2>
    <p>把图像识别接入挑战生命周期、短期凭证、重试语义和审计链路。</p>
    <span class="article-link">开始阅读 →</span>
  </a>
</div>

## 阅读建议

- 如果你关注算法与视觉任务：从第 1 篇开始；
- 如果你关注工程落地与指标：重点阅读第 2 篇；
- 如果你关注协议、服务端信任边界和可观测性：直接阅读第 3 篇。

## 内容边界

本专题讨论授权环境中的任务建模、工程评测和协议设计，不公开第三方产品未公开的接口、签名算法、核心实现或绕过代码。

---

*说明：本文讨论授权范围内的人机验证与图像挑战研究方法；具体产品能力、接口和实现以官方文档、合同及当地法律为准。*
