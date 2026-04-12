# Skills 目录

本目录存放自定义技能（Skills），每个 Skill 是一个独立的模块，用于扩展 Atlas 的能力边界。

---

## 自定义 Skills

### 📝 [ai-article-writer](ai-article-writer/)

**AI 科普文章写作助手 v3.3（公众号专享版）**

- **功能**：生成 AI 科普文章周素材计划，专注于微信公众号平台，深度优化阅读量、分享率、关注转化率
- **包含**：爆款标题库、开篇模板、SCQA 内容结构、传播设计、封面图生成规范、A/B 测试方法、数据复盘模板
- **触发**：生成公众号文章、规划一周公众号素材、优化文章标题/开篇/结构、提升公众号打开率/读完率/分享率
- **版本**：3.3（2026-04-12）
- **参考文件**：
  - `references/topic-selection.md` — 公众号用户画像、选题策略、优先级矩阵
  - `references/content-planning.md` — 周素材规划模板、发布策略
  - `references/writing-techniques.md` — 7 大爆款标题公式、5 种开篇模板、表达技巧
  - `references/image-generation.md` — 封面图/头图/配图/代码截图生成规范
  - `references/quality-check.md` — Fake News 五层检查、发布前质量清单
  - `references/data-tracking.md` — 核心指标体系、A/B 测试、数据复盘模板
  - `references/case-studies.md` — 改造案例演示（技术博客→公众号）

### 🎨 [nano-banana-2](nano-banana-2/)

**Nano Banana 2 — Google Gemini 3.1 Flash Image Preview**

- **功能**：通过 inference.sh CLI 调用 Google Gemini 3.1 Flash 模型生成图片
- **能力**：文生图、图片编辑、多图输入（最多 14 张）、Google Search 信息增强
- **依赖**：inference.sh CLI（`infsh`），需登录并充值
- **触发**：nano banana 2、nanobanana 2、gemini 3.1 flash image、google image generation
- **安装**：`curl -fsSL https://cli.inference.sh | sh && infsh login`
- **注意**：账户余额不足时无法使用，需在 https://app.inference.sh/settings/billing 充值

---

## 系统内置 Skills

以下 Skills 由 OpenClaw 系统内置，无需安装即可使用：

| Skill | 功能 |
|-------|------|
| `clawhub` | ClawHub 技能市场搜索、安装、更新、发布 |
| `coding-agent` | 委托编码任务给 Codex/Claude Code 等编程 Agent |
| `healthcheck` | 主机安全加固和风险配置检查 |
| `node-connect` | 诊断 OpenClaw 节点连接和配对问题 |
| `skill-creator` | 创建、编辑、审核 Agent Skills |
| `taskflow` | 多任务流程编排与管理 |
| `wacli` | 通过 WhatsApp CLI 发送消息、搜索聊天记录 |
| `weather` | 获取天气预报和实时数据（wttr.in / Open-Meteo） |
| `xurl` | X (Twitter) API 工具：发帖、回复、搜索、上传媒体 |
