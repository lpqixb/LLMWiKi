---
type: entity
status: active
created: 2026-11-14
---

# WorkBuddy

> **限定**：以下信息来自接入教程文档，未独立调研产品全貌。

## 概述

WorkBuddy 是一款跨平台桌面 AI 应用（当前版本 5.11.3 见于 macOS），支持 macOS（ARM64 / X64）和 Windows。支持通过自定义供应商接入第三方 OpenAI 兼容服务。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 关键信息

- **官网**：https://www.workbuddy.cn/
- **模型配置文档**：https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model
- **平台支持**：macOS（ARM64 / X64）、Windows
- **第三方接入**：通过设置 → 模型 → 添加模型 → 供应商选"自定义"，填写完整接口地址（如 `https://www.tokenage.ai/v1/chat/completions`）、API Key 和模型名称。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
- **本地配置存储**：`~/.workbuddy/models.json`，不应分享或上传。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 关联

- 实体：[[TokenAge]]
- 主题：[[第三方 AI 应用接入]]

## 待核验

- [ ] 最新版本号和完整功能列表。
- [ ] 是否支持其他第三方 AI 服务提供商。
