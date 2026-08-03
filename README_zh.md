# AI 自定义技能库

[English Version](./README.md)

---

> 针对多个平台的生产级AI与自动化技能，涵盖内容创作、数据导出、工作流自动化与智能任务调度。

**创建与维护者：** [Jeff Yang](https://github.com/j3ffyang)

[![许可证](https://img.shields.io/badge/许可证-MIT-green)](LICENSE)
[![技能总数](https://img.shields.io/badge/技能数量-23-blue)](#平台与技能目录)

---

## 快速导航

请选择您的平台：

| 平台 | 用例 | 技能数量 | 了解详情 |
|-------|-------|-----------|---------|
| **Claude Code** | 云端IDE自动化，快速命令 | 3 | [`claude-code/`](./claude-code/README.md) |
| **OpenClaw** | 工作流自动化，ClawHub注册库 | 13 | [`openclaw/`](./openclaw/README.md) |
| **Hermes** | 代理管理，自动工作流 | 7 | [`hermes/`](./hermes/README.md) |

---

## 技能目录

### Claude Code（3个技能）
扩展 [Claude Code](https://claude.ai/code) IDE，支持自定义快速命令及生产效率工具。

- [`perplexity-downloader`](./claude-code/perplexity-downloader/) — 下载并导出Perplexity对话内容为Markdown格式
- [`readme-i18n`](./claude-code/readme-i18n/) — 同步README.md到简体中文，支持多语言
- [`twitter-bookmarks-exporter`](./claude-code/twitter-bookmarks-exporter/) — 导出X/Twitter书签，附带元数据和媒体链接

### OpenClaw（13个技能）
部署至ClawHub，支持工作流自动化、内容润色、图像和视频生成等。

#### 文章润色
- [`indepth-perspective`](./openclaw/indepth-perspective/) — 构建有说服力、情感丰富的文章框架
- [`blog-polish-zhcn`](./openclaw/blog-polish-zhcn/) — 优化并翻译技术稿至简体中文
- [`blog-polish-en-astro-cn`](./openclaw/blog-polish-en-astro-cn/) — 英文+中文润色，转换为Astro Markdown
- [`blog-polish-eng-single-image`](./openclaw/blog-polish-eng-single-image/) — 英文润色，生成封面图提示
- [`blog-polish-eng-multi-images`](./openclaw/blog-polish-eng-multi-images/) — 多图润色
- [`blog-polish-zhcn-images`](./openclaw/blog-polish-zhcn-images/) — 中文润色，配图提示

#### 图像生成
- [`blog-image-embedder`](./openclaw/blog-image-embedder/) — 生成并插入图片占位符
- [`blog-image-enricher`](./openclaw/blog-image-enricher/) — 添加封面及章节配图

#### 视频生成
- [`image-to-video-gen`](./openclaw/image-to-video-gen/) — 利用Google Veo将图像转为电影短片

#### 新闻 & 内容
- [`ai-newsletter`](./openclaw/ai-newsletter/) — 生成每日AI新闻通讯
- [`ai-newsletter-chn`](./openclaw/ai-newsletter-chn/) — 中文每日AI新闻

#### 特色内容
- [`tibetan-buddhist-product-article-generator`](./openclaw/tibetan-buddhist-product-article-generator/) — 藏传佛事内容
- [`tibetan-cinematic-video`](./openclaw/tibetan-cinematic-video/) — 藏族特色电影

### Hermes（7个技能）
部署至Hermes，支持自动工作流和内容生成。

- [`ai-newsletter-prompt`](./hermes/ai-newsletter-prompt/) — 生成每日AI新闻
- [`ai-newsletter-prompt-chn`](./hermes/ai-newsletter-prompt-chn/) — 中文新闻
- [`five-dynasties-ten-kingdoms-article`](./hermes/five-dynasties-ten-kingdoms-article/) — 历史长文
- [`silk-essay-framework`](./hermes/260620-silk-essay-chn/) — 中国丝绸深度分析框架
- [`markdown-to-minimal-image`](./hermes/260611-md2mini-img/) — 将Markdown文档总结并生成极简白板风格图片（5:2 / 5:4 社交横幅）
- [`luoshenfu-literary-research`](./hermes/260625-luoShenFu/) — 《洛神赋》文学研究专题文章
- [`zhiyanzhai-research`](./hermes/260723-zhiYanZhai/) — 脂砚斋身份考据研究长文（约一万字）

---

## 前置条件
- Claude Code：已安装验证
- OpenClaw CLI：已安装验证
- Hermes CLI：已安装验证

## 安装方法
- 克隆仓库，安装技能
- 通过命令导入技能

## 使用指南
- 调用技能，传入参数
- 查看输入输出定义

## 贡献方式
- 阅读贡献指南
- 提交skill定义

## 许可证
- 遵循MIT协议

---