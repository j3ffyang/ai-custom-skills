# Hermes技能

> 面向Hermes（https://hermes.ai）智能体平台的生产级技能，专为自主工作流自动化和智能任务编排设计。

**← [返回主目录](../README.md)**

---

## 可用技能

| 技能 | 描述 | 语言 |
|-------|-----------|--------|
| [`ai-newsletter-prompt`](./ai-newsletter-prompt/) | 生成每日AI新闻通讯，来源于实时网络 | 英文 |
| [`ai-newsletter-prompt-chn`](./ai-newsletter-prompt-chn/) | 为中文用户生成每日AI新闻通讯 | 中文 |
| [`five-dynasties-ten-kingdoms-article`](./five-dynasties-ten-kingdoms-article/) | 研究并撰写五代十国（公元907–979）时期的时间线长文 | 中文 |
| [`silk-essay-framework`](./260620-silk-essay-chn/) | 关于中国丝绸纺织品（绫罗绸缎）的深度文章框架，结合历史、技术与文学分析 | 中文 |
| [`markdown-to-minimal-image`](./260611-md2mini-img/) | 将Markdown文档总结并生成极简白板风格图片（支持 5:2 / 5:4 社交横幅） | 中文/英文 |
| [`luoshenfu-literary-research`](./260625-luoShenFu/) | 《洛神赋》文学研究专题文章，涵盖文学、历史与哲学维度 | 中文 |
| [`zhiyanzhai-research`](./260723-zhiYanZhai/) | 脂砚斋身份考据研究长文（约一万字），探讨《红楼梦》匿名批者 | 中文 |

---

## 前提条件

- [Hermes CLI](https://hermes.ai/docs/cli) 已安装并验证
- Hermes 代理运行环境（本地或托管）
- API访问权限（具体skill需求）:
  - 网络调研：`BRAVE_API_KEY`，`FIRECRAWL_API_KEY`

---

## 安装指南

### 方式一：从仓库克隆

```bash
git clone https://github.com/j3ffyang/ai-custom-skills.git
cd ai-custom-skills/hermes
# 安装技能（局部）
hermes skill install ./ai-newsletter-prompt
```

### 方式二：从本地目录安装

```bash
hermes skill install ./你的技能目录
```

---

## 使用指南

每个技能可通过 Hermes CLI 或代理环境调用：

```bash
hermes run ai-newsletter-prompt
```

或者带参数：

```bash
hermes run ai-newsletter-prompt --input 'search_query="最新AI突破" target_news_count=15'
```

在Hermes代理工作流中调用：

```
使用该技能生成每日新闻简报。
```

查看详细的输入输出契约和工作流配置：`SKILL.md`文件

---

## 环境变量配置

大部分技能需要第三方API密钥。请提前配置：

```bash
export BRAVE_API_KEY="你的API密钥"
export FIRECRAWL_API_KEY="你的API密钥"
```

在生产环境中，建议在Hermes配置或密钥管理中设置。

---

## 贡献指南

详见 [`../CONTRIBUTING.md`](../CONTRIBUTING.md) 文件。

## 许可证

本项目遵循MIT许可证，具体条款见 LICENSE 文件。