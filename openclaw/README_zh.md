# OpenClaw技能

> 面向[OpenClaw](https://openclaw.ai)工作流自动化平台的生产级技能，已发布至[ClawHub](https://clawhub.ai)注册库。

**← [返回主目录](../README.md)**

---

## 技能分类

### 文章框架
- [`indepth-perspective`](./indepth-perspective/) — 建设说服力强、情感层叠的文章的可复用框架

### 文章润色
- [`blog-polish-zhcn`](./blog-polish-zhcn/) — 打磨及翻译成简体中文
- [`blog-polish-en-astro-cn`](./blog-polish-en-astro-cn/) — 英文+中文润色，转为Astro Markdown格式
- [`blog-polish-eng-single-image`](./blog-polish-eng-single-image/) — 英文润色，生成封面图提示
- [`blog-polish-eng-multi-images`](./blog-polish-eng-multi-images/) — 英文润色，生成封面图及部分段落配图
- [`blog-polish-zhcn-images`](./blog-polish-zhcn-images/) — 中文润色，生成配图提示

### 图像生成
- [`blog-image-embedder`](./blog-image-embedder/) — 生成并嵌入图片占位符
- [`blog-image-enricher`](./blog-image-enricher/) — 在 Markdown 添加头部和章节配图

### 视频生成
- [`image-to-video-gen`](./image-to-video-gen/) — 使用 Google Veo 将图片转为电影短片

### 新闻内容
- [`ai-newsletter`](./ai-newsletter/) — 生成每日AI新闻通讯
- [`ai-newsletter-chn`](./ai-newsletter-chn/) — 生成中文每日AI新闻

### 专题内容
- [`tibetan-buddhist-product-article-generator`](./tibetan-buddhist-product-article-generator/) — 藏传佛事产品文章生成
- [`tibetan-cinematic-video`](./tibetan-cinematic-video/) — 藏族特色电影视频生成

---

## 前置条件
- [OpenClaw CLI](https://openclaw.ai) 已安装并验证
- ClawHub 账号（安装技能）
- 相关API密钥：OpenAI DALL-E-3、Google Veo、Gemini 2.5

---

## 安装方法

### 从ClawHub注册库

```bash
openclaw skill install <技能名>
# 示例
openclaw skill install blog-polish-zhcn
```

### 从本地目录安装

```bash
openclaw skill install ./技能目录
```

---

## 使用说明
- 通过命令行调用，示例：

```bash
# 交互式
openclaw run blog-polish-zhcn
# 传参
openclaw run blog-polish-zhcn --input draftPath=./my-draft.md outputDir=./out
```
- 查看各技能的 `SKILL.md` 了解详细配置。

---

## 贡献指南
- 详细见 [`CONTRIBUTING.md`](../CONTRIBUTING.md)
- 新建技能：创建文件夹，撰写 `SKILL.md`、`README.md`，本地测试，提交PR。

---

## 许可证
- 遵循MIT协议，详见LICENSE。