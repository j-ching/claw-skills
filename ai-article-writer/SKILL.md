---
name: ai-article-writer
description: 生成 AI 科普文章周素材计划，专注于微信公众号平台，深度优化阅读量、分享率、关注转化率。包含爆款标题库、开篇模板、传播设计等完整增长策略。Use when: 用户要求生成公众号文章、规划一周公众号素材、优化文章标题/开篇/结构、生成公众号封面图、提升公众号打开率/读完率/分享率、进行公众号 A/B 测试或数据复盘。NOT for: 其他平台（小红书/抖音/知乎）的专属内容生成、非 AI 领域的文章写作。
metadata:
  version: 3.3
  lastUpdated: 2026-04-12
---

# AI 科普文章写作助手 v3.3（公众号专享版）

## 核心价值

帮助 AI 技术创作者批量生产爆款公众号文章，通过阅读量倍增策略和社交传播设计，全面提升打开率、分享率、关注转化率。

## 工作流程

```
用户需求 → 主题确定 → 内容规划 → 文章生成 → 插图生成 → 质量检查 → 发布优化
```

### 步骤 1：确定题材方向

**方式 A：用户指定主题** — 询问技术领域、目标读者、内容调性、实操要求（见 [references/topic-selection.md](references/topic-selection.md)）

**方式 B：自动选择热点** — 按优先级筛选：
- **海外渠道（优先）**：Hacker News、arXiv、GitHub Trending、Product Hunt、Twitter/X
- **国内渠道（补充）**：知乎、微信公众号、掘金、V2EX

**选题优先级**（基于互联网热度排序）：
- **⭐⭐⭐⭐⭐ 热门事件/重磅发布**：Hacker News 首页、Twitter 热议
- **⭐⭐⭐⭐⭐ 框架对比**：GitHub Stars、社区讨论热度
- **⭐⭐⭐⭐ 新框架/工具介绍**：GitHub Trending、Product Hunt
- **⭐⭐⭐⭐ 快速上手教程**：搜索需求、社区问答热度
- **⭐⭐⭐ 架构概览**：技术博客引用
- **⭐⭐ 原理解析**：arXiv 论文引用
- **⭐ 配置细节**：文档搜索
- **黄金比例**：70% 浅显易懂 + 30% 技术深度

**选题范围**：大语言模型 / AI Agent / RAG 系统 / 多模态 AI / Agentic RL / 强化学习 / 深度学习 / 模型训练与微调 / AI 评测 / 周边框架（PyTorch、TensorFlow、Ray、DeepSpeed、vLLM 等）

详见 [references/topic-selection.md](references/topic-selection.md)。

### 步骤 2：规划周素材结构

按标准化模板规划一周 7 天内容，每天 2 篇（共 14 篇），包含爆款标题公式编号、开篇模板、传播设计。发布时间：工作日 7:30-8:30 / 12:00-13:00 / 21:00-22:00。

详见 [references/content-planning.md](references/content-planning.md)。

### 步骤 3：生成文章

每篇文章 3000-8000 字（5000 字最佳），采用 SCQA 结构模型：
1. 引言（痛点引入，300 字）
2. 背景知识（500 字）
3. 核心方案（2000 字，3-5 小节）
4. 实操步骤（1500 字，带代码）
5. 性能对比（500 字，数据表格）
6. 常见问题（500 字，FAQ）
7. 总结与延伸（200 字）
8. 结尾引导（行动号召 + 讨论话题）

标题公式、开篇模板、表达技巧详见 [references/writing-techniques.md](references/writing-techniques.md)。

### 步骤 4：生成封面图

**强制要求**：每篇文章必须有一张封面图（1536x1024，3:2 比例），蓝紫渐变背景 (#667eea → #764ba2)。

**有图片生成工具时**：用 ImageGen/DALL-E 等工具生成，保存到 `images/` 目录，文章开头引用。

**无图片生成工具时**：为每篇文章构建封面 Prompt，保存到 `cover-images.md`，提示用户用外部工具生成。

详见 [references/image-generation.md](references/image-generation.md)。

### 步骤 5：质量检查

发布前必须通过：
- **真实性核查**：事件/归属/时间/数据/表述完整性（五层 Fake News 检查）
- **内容完整性**：实操步骤、可运行代码、预期结果、FAQ、配图
- **平台适配**：标题 20-26 字、段落≤5 行、每 500-800 字小标题、封面图

详见 [references/quality-check.md](references/quality-check.md)。

### 步骤 6：数据追踪与优化

核心指标：打开率（>15% 优秀）、读完率（>70% 优秀）、分享率（>5% 优秀）、在看率（>2% 优秀）。

A/B 测试标题、封面、开篇，持续迭代。复盘模板见 [references/data-tracking.md](references/data-tracking.md)。

## 输出规范

- **字数**：3000-8000 字，阅读 8-15 分钟
- **配图**：5-10 张（900x383px 头图 + 文中配图）
- **代码块**：3-5 个完整示例
- **表格**：2-3 个对比/总结表
- **引用**：3-5 处权威来源
- **排版**：15-16px 字号、1.6-1.8 倍行距、段距空一行

**⚠️ 不生成**"粉丝福利"（关键词回复领资料）和"互动话题"（选择题+抽奖），由发布者自行处理。

## 参考文件索引

| 文件 | 内容 |
|------|------|
| [topic-selection.md](references/topic-selection.md) | 公众号用户画像、选题策略、优先级矩阵 |
| [content-planning.md](references/content-planning.md) | 周素材规划模板、发布计划 |
| [writing-techniques.md](references/writing-techniques.md) | 爆款标题公式库、开篇模板、SCQA 结构、表达技巧 |
| [image-generation.md](references/image-generation.md) | 封面图/插图/代码截图生成规范 |
| [quality-check.md](references/quality-check.md) | Fake News 五层检查、内容质量清单 |
| [data-tracking.md](references/data-tracking.md) | 指标体系、A/B 测试、数据复盘模板 |
| [case-studies.md](references/case-studies.md) | 改造案例演示（技术博客→公众号） |
