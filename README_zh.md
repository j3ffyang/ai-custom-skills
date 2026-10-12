# AI 自定义技能库

> 针对多个平台的生产级 AI 与自动化技能，涵盖内容创作、数据导出、工作流自动化与智能任务调度。

**创建与维护者：** [Jeff Yang](https://github.com/j3ffyang)

[![许可证](https://img.shields.io/badge/许可证-MIT-green)](LICENSE) [![技能总数](https://img.shields.io/badge/技能数量-23-blue)](#平台与技能目录)

---
[English Version](./README.md) | [中文版本](./README_zh.md)

## 快速导航

**请选择您的平台：**

| 平台 | 用例 | 技能数量 | 了解详情 |
|----------|----------|--------|------------|
| **OpenCode** | 会话技能，通过 `skills.paths` 加载 | 20+ | [`ai-thoughts/.opencode/skills/`](https://github.com/j3ffyang/ai-thoughts/tree/main/.opencode/skills) |
| **Hermes** | 代理编排，自动工作流 | 7 | [`hermes/`](./hermes/README.md) |
| **OpenClaw** | 工作流自动化，ClawHub 注册库 | 13 | [`openclaw/`](./openclaw/README.md) |
| **Claude Code** | 云端 IDE 自动化，快速命令 | 3 | [`claude-code/`](./claude-code/README.md) |

---

## 目录

- [快速导航](#快速导航)
- [平台与技能目录](#平台与技能目录)
- [前置条件](#前置条件)
- [安装方法](#安装方法)
- [贡献方式](#贡献方式)
- [项目结构](#项目结构)
- [贡献者](#贡献者)
- [许可证](#许可证)
- [相关链接](#相关链接)

---

## 平台与技能目录

### OpenCode（托管于 [ai-thoughts](https://github.com/j3ffyang/ai-thoughts)）

OpenCode 没有公开的技能注册库，因此**不从本仓库发布**。它的技能与工作内容一同存放在姊妹仓库 [`ai-thoughts/.opencode/skills/`](https://github.com/j3ffyang/ai-thoughts/tree/main/.opencode/skills)（20+ 个技能）中，并通过 `~/.config/opencode/opencode.jsonc` 里的 `skills.paths` 在每个 OpenCode 会话中加载。

**📖 来源：** [`j3ffyang/ai-thoughts` · `.opencode/skills/`](https://github.com/j3ffyang/ai-thoughts/tree/main/.opencode/skills)

---

### Hermes（7 个技能）
部署至 Hermes 代理平台，用于自动工作流编排和内容生成。

- **[`ai-newsletter-prompt`](./hermes/ai-newsletter-prompt/)** — 基于最新网络来源生成每日 AI 新闻通讯
- **[`ai-newsletter-prompt-chn`](./hermes/ai-newsletter-prompt-chn/)** — 为中文读者生成每日 AI 新闻通讯
- **[`five-dynasties-ten-kingdoms-article`](./hermes/five-dynasties-ten-kingdoms-article/)** — 研究并撰写一篇以时间线驱动的五代十国（约 907–979 年）长篇中文文章
- **[`silk-essay-framework`](./hermes/260620-silk-essay-chn/)** — 中国丝绸（绫罗绸缎）深度文章框架，含历史、技术与文学分析
- **[`markdown-to-minimal-image`](./hermes/260611-md2mini-img/)** — 总结 Markdown 文档并生成极简白板风格图片（5:2 / 5:4 社交横幅）
- **[`luoshenfu-literary-research`](./hermes/260625-luoShenFu/)** — 研究并撰写《洛神赋》的综合分析文章
- **[`zhiyanzhai-research`](./hermes/260723-zhiYanZhai/)** — 考据《红楼梦》匿名评点者脂砚斋的身份，撰写约一万字的文章

**📖 平台指南：** [`hermes/README.md`](./hermes/README.md)

---

### OpenClaw（13 个技能）
部署至 [ClawHub](https://clawhub.ai) 注册库，用于工作流自动化、内容润色、媒体生成与藏传佛教内容工作流。

#### 写作与内容润色
- **[`indepth-perspective`](./openclaw/indepth-perspective/)** — 构建有说服力、情感层次丰富的文章框架
- **[`blog-polish-zhcn`](./openclaw/blog-polish-zhcn/)** — 优化并翻译技术稿至简体中文
- **[`blog-polish-en-astro-cn`](./openclaw/blog-polish-en-astro-cn/)** — 润色为英文 + 中文，并转换为 Astro markdown
- **[`blog-polish-eng-single-image`](./openclaw/blog-polish-eng-single-image/)** — 润色英文博客并生成封面图提示
- **[`blog-polish-eng-multi-images`](./openclaw/blog-polish-eng-multi-images/)** — 润色英文博客并生成封面图及各章节配图提示
- **[`blog-polish-zhcn-images`](./openclaw/blog-polish-zhcn-images/)** — 润色中文博客并生成配图提示

#### 图像生成
- **[`blog-image-embedder`](./openclaw/blog-image-embedder/)** — 生成并将图片占位符嵌入博客 markdown
- **[`blog-image-enricher`](./openclaw/blog-image-enricher/)** — 为任意 markdown 文件添加头部及章节配图

#### 视频生成
- **[`image-to-video-gen`](./openclaw/image-to-video-gen/)** — 使用 Google Veo 将图像生成电影级 MP4 视频

#### 新闻与内容
- **[`ai-newsletter`](./openclaw/ai-newsletter/)** — 基于网络来源生成每日 AI 新闻通讯
- **[`ai-newsletter-chn`](./openclaw/ai-newsletter-chn/)** — 生成简体中文每日 AI 新闻通讯

#### 特色内容
- **[`tibetan-buddhist-product-article-generator`](./openclaw/tibetan-buddhist-product-article-generator/)** — 生成含配图的藏传佛教产品文章
- **[`tibetan-cinematic-video`](./openclaw/tibetan-cinematic-video/)** — 生成原汁原味的藏地电影短片

**📖 平台指南：** [`openclaw/README.md`](./openclaw/README.md)

---

### Claude Code（3 个技能）
扩展 [Claude Code](https://claude.ai/code) IDE，支持自定义快速命令与生产力自动化。

- **[`perplexity-downloader`](./claude-code/perplexity-downloader/)** — 下载并导出 Perplexity.ai 对话为 Markdown
- **[`readme-i18n`](./claude-code/readme-i18n/)** — 同步 README.md 到简体中文，支持国际化
- **[`twitter-bookmarks-exporter`](./claude-code/twitter-bookmarks-exporter/)** — 导出 X/Twitter 书签，附带元数据与媒体链接

**📖 平台指南：** [`claude-code/README.md`](./claude-code/README.md)

---

## 前置条件

### 面向 Claude Code
- 已安装并完成认证的 [Claude Code](https://claude.ai/code)

### 面向 OpenClaw
- 已安装并完成认证的 [OpenClaw CLI](https://openclaw.ai)
- ClawHub 账户（用于安装注册库技能）
- 按需的 API 访问权限：OpenAI DALL-E-3、Google Veo、Gemini 2.5 Flash

### 面向 Hermes
- 已安装并完成认证的 [Hermes CLI](https://hermes.ai)
- Hermes 代理运行时
- 按需的 API 访问权限：`BRAVE_API_KEY`、`FIRECRAWL_API_KEY`

---

## 安装方法

### 克隆仓库

```bash
git clone https://github.com/j3ffyang/ai-custom-skills.git
cd ai-custom-skills
```

### 安装指定技能

进入目标平台目录：

```bash
# Claude Code 技能
cd claude-code/
# 将 .claude/ 文件夹复制到你的项目（见 claude-code/README.md）

# OpenClaw 技能
cd openclaw/
openclaw skill install ./blog-polish-zhcn

# Hermes 技能
cd hermes/
hermes skill install ./ai-newsletter-prompt
```

各平台的详细安装说明请见**平台专属 README 文件**。

---

## 贡献方式

### 通用准则

见 [`CONTRIBUTING.md`](./CONTRIBUTING.md)，其中包含：
- 如何添加新技能
- 技能结构与 SKILL.md 格式
- 测试清单
- PR 提交流程

### 平台专属贡献指南

每个平台都有各自的贡献指南：
- **Claude Code：** [`claude-code/README.md`](./claude-code/README.md)
- **OpenClaw：** [`openclaw/README.md`](./openclaw/README.md)
- **Hermes：** [`hermes/CONTRIBUTING.md`](./hermes/CONTRIBUTING.md)

---

## 项目结构

```
ai-custom-skills/
├── README.md                    ← 你在这里
├── CONTRIBUTING.md              ← 通用贡献指南
├── LICENSE                      ← MIT 许可证
│
├── claude-code/                 ← Claude Code IDE 技能
│   ├── README.md
│   ├── perplexity-downloader/
│   ├── readme-i18n/
│   └── twitter-bookmarks-exporter/
│
├── openclaw/                    ← OpenClaw 工作流技能
│   ├── README.md
│   ├── ai-newsletter/
│   ├── blog-polish-zhcn/
│   ├── image-to-video-gen/
│   └── ...（另外 11 个）
│
└── hermes/                      ← Hermes 代理技能（7）
    ├── README.md
    ├── CONTRIBUTING.md
    ├── ai-newsletter-prompt/
    ├── ai-newsletter-prompt-chn/
    ├── five-dynasties-ten-kingdoms-article/
    ├── 260611-md2mini-img/
    ├── 260620-silk-essay-chn/
    ├── 260625-luoShenFu/
    └── 260723-zhiYanZhai/
```

---

## 贡献者

| 姓名 | 角色 | GitHub |
|------|------|--------|
| **Jeff Yang** | 创建者、设计者与维护者 | [@j3ffyang](https://github.com/j3ffyang) |

本项目整合了最初分散在三个独立仓库中的技能。欢迎贡献与反馈！准则见 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## 许可证

本项目基于 [MIT 许可证](LICENSE) 授权。

各个技能可在其 `SKILL.md` 或 README 文件中声明各自的许可证。

---

## 相关链接

- **GitHub：** [j3ffyang/ai-custom-skills](https://github.com/j3ffyang/ai-custom-skills)
- **Claude Code：** https://claude.ai/code
- **OpenClaw：** https://openclaw.ai
- **ClawHub 注册库：** https://clawhub.ai
- **Hermes：** https://hermes.ai
