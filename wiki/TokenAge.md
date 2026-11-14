---
type: entity
status: active
created: 2026-11-14
---

# TokenAge

> **限定**：以下信息来自教程配置文档，未实际测试调用或计费。

## 概述

TokenAge 是一个提供 OpenAI 兼容 API 的第三方 AI 服务平台，可通过 API Key 和模型 ID 接入多种桌面应用（如 DeepSeek Harness、WorkBuddy）。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]、[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 接口信息

| 项目 | 值 |
| --- | --- |
| 官网 | https://www.tokenage.ai/ |
| 文档 | https://www.tokenage.ai/docs |
| Base URL | `https://www.tokenage.ai/v1` |
| Chat Completions 端点 | `/v1/chat/completions` |
| 协议 | OpenAI Chat Completions 兼容 |

来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]、[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 已提及模型

- `gpt-6.1-terra`：在 TokenAge 模型广场可见，具体可用性和价格以平台页面为准。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 已支持的应用

- [[DeepSeek Harness]]：通过自定义模型 API 接入，填写 Base URL。
- [[WorkBuddy]]：通过自定义供应商接入，填写完整聊天接口地址。

## 待核验

- [ ] 完整的模型列表和定价结构。
- [ ] 各模型的工具调用、图片输入、思考模式等能力支持情况。
- [ ] 与原始 OpenAI API 的兼容性程度。
