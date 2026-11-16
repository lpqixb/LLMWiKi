---
type: source-summary
status: active
source: raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程.md
published: 2026-11-14
accessed: 2026-11-14
---

# 来源摘要：WorkBuddy 接入 TokenAge 简明教程

## 来源

- 原始文件：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
- 原始 URL：https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model
- 发布日期：2026-11-14
- 访问日期：2026-11-14

## 核心摘要

本文整理如何将 TokenAge 的 OpenAI 兼容 API 接入 WorkBuddy 桌面应用（v5.11.3），包括下载、准备 API Key 和模型 ID、添加自定义供应商模型、配置接口地址和验证调用的步骤。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 关键主张与证据

1. WorkBuddy 提供 macOS（ARM64 / X64）和 Windows 安装包，从官网下载。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
2. TokenAge 的聊天接口地址为 `https://www.tokenage.ai/v1/chat/completions`；WorkBuddy 的"接口地址"字段需要填写完整路径。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
3. 在 WorkBuddy 中配置路径：设置 → 模型 → 添加模型 → 供应商选"自定义"，填写接口地址、API Key、模型名称。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
4. 与 Harness 的差异：Harness 填 `/v1` 根地址，WorkBuddy 填完整 `/v1/chat/completions` 地址。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]] 与 [[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
5. 配置和密钥保存在本机 `~/.workbuddy/models.json`，不应分享或上传。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 关联

- 实体：[[TokenAge]]
- 实体：[[WorkBuddy]]
- 参见：[[DeepSeek Harness 接入 TokenAge 简明教程]]（来源摘要）

## 冲突与限定

- 截图来自 macOS 上的 WorkBuddy 5.11.3；不同版本界面可能不同。未实际添加密钥或测试付费调用。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
