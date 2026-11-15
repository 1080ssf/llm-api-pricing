# 全球大模型 API 官方价格汇总（LLM API Pricing）

> OpenAI GPT、Anthropic Claude、Google Gemini、xAI Grok、Mistral、DeepSeek、智谱 GLM、Kimi、MiniMax、通义千问、豆包等 **大模型 API 官方价格对比表**，每百万 tokens 输入 / 输出 / 缓存价格一目了然，每条都附官方价格页链接。
>
> A side-by-side comparison of official LLM API prices (per 1M tokens) for GPT, Claude, Gemini, Grok, Mistral, DeepSeek, GLM, Kimi, MiniMax and more, with links to every official pricing page.

**数据核对日期：2026-11-15。** 各家调价频繁，下单前请点「来源」链接以官网为准；发现过期欢迎提 Issue / PR。

- 单位：**每 100 万 tokens**。海外厂商为美元（USD），国内厂商为人民币（CNY），不做汇率换算。
- 「缓存」指缓存命中（cache hit / cached input）的输入价；「—」表示官方页未单列。
- 只收录当前主力文本模型；已弃用、即将下线的不列。

## 目录

- [海外厂商（USD）](#海外厂商usd)：OpenAI · Anthropic Claude · Google Gemini · xAI Grok · Mistral
- [国内厂商（CNY）](#国内厂商cny)：DeepSeek · 智谱 GLM · 月之暗面 Kimi · MiniMax · 通义千问 · 豆包
- [怎么看这张表](#怎么看这张表)
- [相关项目](#相关项目)

## 海外厂商（USD）

### OpenAI

| 模型 | 输入 | 缓存 | 输出 | 备注 |
|---|---:|---:|---:|---|
| gpt-6-astra | 10.00 | 1.00 | 50.00 | 旗舰 |
| gpt-6.1-sol | 2.00 | 0.10 | 10.00 | |
| gpt-6.1-terra | 1.00 | 0.05 | 5.00 | |
| gpt-6-luna | 0.10 | 0.01 | 0.50 | 小模型 |
| gpt-5.5 | 5.00 | 0.50 | 30.00 | 输入 < 272K |
| gpt-5.4-mini | 0.75 | 0.075 | 4.50 | |
| gpt-5.4-nano | 0.20 | 0.02 | 1.25 | |
| o3 | 2.00 | 0.50 | 8.00 | 推理模型 |

来源：[OpenAI API Pricing](https://developers.openai.com/api/docs/pricing)（Standard 档，短上下文）

### Anthropic Claude

| 模型 | 输入 | 缓存 | 输出 | 上下文 | 备注 |
|---|---:|---:|---:|---|---|
| claude-fable-5-2 | 8.00 | 0.20 | 40.00 | 1M | 最强 |
| claude-opus-5-5 | 4.00 | 0.20 | 20.00 | 1M | |
| claude-sonnet-5-5 | 2.00 | 0.10 | 10.00 | 1M | |
| claude-haiku-5-5 | 0.10 | — | 0.50 | 1M | 输入 ≤ 100K；超过后 0.50 / 2.50 |

来源：[Claude API Pricing](https://platform.claude.com/docs/en/about-claude/pricing)（Claude API 官方价；Bedrock / Vertex 另行定价）

### Google Gemini

| 模型 | 输入 | 缓存 | 输出 | 备注 |
|---|---:|---:|---:|---|
| Gemini 4 Carbon | 2.00 | 0.10 | 10.00 | 2026-12-01 起 4.00 / 0.20 / 20.00；无免费档 |
| Gemini 4 Hydrogen | 1.50 | 0.075 | 7.50 | 有免费档 |
| Gemini 3.8 Flash | 0.75 | 0.075 | 3.75 | 2027-01-01 起 1.50 / 0.15 / 7.50 |
| Gemini 3.5 Flash-Lite | 0.30 | 0.03 | 2.50 | |
| Gemini 3.1 Flash-Lite | 0.25 | 0.025 | 1.50 | 文本 / 图片 / 视频输入 |

来源：[Gemini API Pricing](https://aistudio.google.com/docs/pricing)（付费档；缓存另有按小时的存储费）

### xAI Grok

| 模型 | 输入 | 缓存 | 输出 | 上下文 | 备注 |
|---|---:|---:|---:|---|---|
| grok-4.7 | 2.00 | 0.50 | 6.00 | 500K | 提示 ≥ 200K 时 4.00 / 1.00 / 12.00 |
| grok-4.3 | 1.25 | 0.20 | 2.50 | 1M | 提示 ≥ 200K 时翻倍 |
| grok-build-0.1 | 1.00 | 0.20 | 2.00 | 256K | 编程 |

来源：[xAI Models and Pricing](https://docs.x.ai/docs/models)

### Mistral

| 模型 | 输入 | 输出 | 备注 |
|---|---:|---:|---|
| Mistral Large 4 | 0.70 | 2.10 | |
| Mistral Small 4 | 0.15 | 0.60 | |
| Codestral | 0.30 | 0.90 | 编程 |
| Ministral 3 8B | 0.15 | 0.15 | |

来源：[Mistral Pricing](https://docs.mistral.ai/inference/pricing)（Batch 半价；缓存输入最多省 90%）

## 国内厂商（CNY）

### DeepSeek

| 模型 | 输入 | 缓存 | 输出 | 上下文 | 备注 |
|---|---:|---:|---:|---|---|
| deepseek-v4-pro | 9.0 | 0.30 | 27.0 | 1M | 高峰价；闲时 4.5 / 0.15 / 13.5 |
| deepseek-flash（V4.1 Flash） | 2 | 0.04 | 8 | 1M | 高峰价；闲时 1 / 0.02 / 4；支持图片理解 |

高峰时段：工作日 9:00–12:00、14:00–18:00（北京时间），其余时间与节假日按闲时半价。提供 OpenAI 兼容（`https://api.deepseek.com`）和 Anthropic 兼容（`https://api.deepseek.com/anthropic`）两种接口。

来源：[DeepSeek 模型与价格](https://api-docs.deepseek.com/zh-cn/quick_start/pricing)

### 智谱 GLM

| 模型 | 输入 | 缓存 | 输出 | 上下文 |
|---|---:|---:|---:|---|
| glm-5.3 | 8 | 2 | 28 | 1M |
| glm-5.3-flash | 0.8 | 0.23 | 2.8 | |

来源：[智谱开放平台价格](https://open.bigmodel.cn/pricing)

### 月之暗面 Kimi

| 模型 | 输入 | 缓存 | 输出 |
|---|---:|---:|---:|
| kimi-k3.1-pro | 13 | 1.3 | 68 |

来源：[Kimi 开放平台价格](https://platform.moonshot.cn/docs/pricing/chat)

### MiniMax

| 模型 | 输入 | 缓存 | 输出 | 备注 |
|---|---:|---:|---:|---|
| MiniMax-M3 | 2.10 | 0.42 | 8.40 | 输入 ≤ 512K（已含官方「永久五折」）；超过后 4.20 / 0.84 / 16.80 |
| MiniMax-M3.1-Flash | 1.00 | 0.10 | 4.00 | |

优先服务（`service_tier: priority`）为标准价 1.5 倍。来源：[MiniMax 价格](https://platform.minimax.cn/docs/guides/pricing)

### 价格待核实（只给官方入口）

以下厂商的官方价格页为动态渲染，本次未能直接读到数字；第三方转载口径不一，为避免误导暂不列价格：

| 厂商 | 主力模型 | 官方价格页 |
|---|---|---|
| 阿里云百炼（通义千问） | qwen4-max-preview、qwen3.7-plus、qwen3.8-flash（均 1M 上下文） | [模型列表与价格](https://help.aliyun.com/zh/model-studio/models) |
| 火山方舟（豆包） | Doubao 系列 | [模型价格](https://docs.volcengine.com/docs/82379/1544106) |

欢迎附官方截图提 PR 补全。

## 怎么看这张表

1. **只看输入价会被坑**：AI 编程、长对话场景里输入 token 远多于输出，**缓存价**往往决定最终账单。会话越长，缓存命中越重要。
2. **注意阶梯价**：Gemini、Grok、Claude Haiku、MiniMax 都有「提示超过 X tokens 后单价翻倍」的规则；DeepSeek 有高峰 / 闲时价。
3. **限时价会过期**：Gemini 4 Carbon、Gemini 3.8 Flash 当前是限时价，表里已标出恢复原价的日期。
4. **推理模型的输出包含思考 token**：同样一句回答，开深度思考时输出 token 可能多好几倍。
5. **按任务算成本，不按单价算**：便宜模型如果需要多轮重试才能完成任务，未必更省。

## 相关项目

- [claude-code-codex-api-config-cn](https://github.com/1080ssf/claude-code-codex-api-config-cn)：Claude Code / Codex / Cline 等工具接入第三方 API 的配置教程
- [claude-md-agents-md-templates-cn](https://github.com/1080ssf/claude-md-agents-md-templates-cn)：CLAUDE.md / AGENTS.md 中文模板与省 token 技巧
- 想用更低价格调用 DeepSeek / GLM / Kimi？可以看看 [Imagio](https://imagio.site)（OpenAI 与 Anthropic 协议兼容，按量计费）。交流群：QQ **1125429694**

## 贡献

价格以**官方价格页**为准。提 PR 时请附上官方链接和核对日期，第三方转载、聚合平台报价不收。

## 许可

数据与文字：CC BY 4.0；如有代码：MIT。
