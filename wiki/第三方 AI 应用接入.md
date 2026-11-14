---
type: topic
status: active
created: 2026-11-14
---

# 第三方 AI 应用接入

> **限定**：以下信息来自两份接入教程文档，未独立验证各应用的完整功能。

## 概述

多款桌面 AI 应用支持通过自定义接口接入第三方 OpenAI 兼容 API 服务（如 [[TokenAge]]），使用户能在一个客户端中调用多个提供商的模型。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]、[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 常见接入模式

两种应用的配置路径不同，但核心要素一致：

| 要素 | [[DeepSeek Harness]] | [[WorkBuddy]] |
| --- | --- | --- |
| 配置入口 | 设置 → 模型 → 添加模型提供商 → 自定义模型 API | 设置 → 模型 → 添加模型 → 供应商选"自定义" |
| 接口地址格式 | Base URL（如 `https://www.tokenage.ai/v1`） | 完整聊天端点（如 `https://www.tokenage.ai/v1/chat/completions`） |
| API 协议 | OpenAI Chat Completions | 通过"自定义协议"开关控制 |
| 本地密钥存储 | 应用内配置 | `~/.workbuddy/models.json` |

来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]、[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]

## 关键注意事项

1. **接口地址层级差异**：不同应用对"接口地址"的定义不同——有的需要 Base URL，有的需要完整端点路径。填写前需确认应用提示。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]、[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
2. **模型能力匹配**：添加模型后，需按实际能力手动开启"工具调用"、"图片输入"、"思考模式"等功能。来源：[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
3. **安全**：API Key 保存在本地，不应分享或上传配置文件；输入内容会发送至第三方服务，需确认其服务协议和隐私政策。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]、[[raw/2026-11-14-WorkBuddy 接入 TokenAge 简明教程]]
4. **社区插件**：部分应用支持社区插件市场（如 Harness 的 DSH Market），安装前应核对来源和兼容性。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]

## 关联

- 实体：[[TokenAge]]
- 实体：[[DeepSeek Harness]]
- 实体：[[WorkBuddy]]

## 待核验

- [ ] 更多桌面 AI 应用（如 Cursor、Claude Desktop 等）的自定义模型接入方式。
- [ ] 不同提供商 API 的协议兼容性差异（如流式响应、工具调用格式）。
