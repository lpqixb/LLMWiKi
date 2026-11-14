---
type: source-summary
status: active
source: raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程.md
published: 2026-11-14
accessed: 2026-11-14
---

# 来源摘要：DeepSeek Harness 接入 TokenAge 简明教程

## 来源

- 原始文件：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]
- 原始 URL：https://www.deepseek.com/zh/download/
- 发布日期：2026-11-14
- 访问日期：2026-11-14

## 核心摘要

本文整理如何将 TokenAge 的 OpenAI 兼容 API 接入 DeepSeek Harness 桌面应用，包括下载、配置自定义模型提供商、添加模型和验证调用的步骤，并介绍了可选社区插件 DSH Market 和 dsh-context 的安装。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]

## 关键主张与证据

1. DeepSeek Harness 桌面端支持 macOS（Apple 芯片，macOS 13+）和 Windows，从官网下载页获取。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]
2. TokenAge 提供 OpenAI Chat Completions 兼容接口，Base URL 为 `https://www.tokenage.ai/v1`。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]
3. 在 Harness 中配置路径：设置 → 模型 → 添加模型提供商 → 自定义模型 API，填写 Provider ID、显示名称、API 地址、协议和密钥，再添加模型并创建。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]
4. Harness 表单中的 API 地址使用 `/v1` 根地址，不是完整的 `/v1/chat/completions` 路径。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]
5. DSH Market 是社区插件市场，dsh-context 提供上下文用量可视化；两者是第三方插件，安装前应核对来源。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]

## 关联

- 实体：[[TokenAge]]
- 实体：[[DeepSeek Harness]]
- 参见：[[WorkBuddy 接入 TokenAge 简明教程]]（来源摘要）

## 冲突与限定

- 本文基于 2026-11-14 的官网资料与本机界面整理，版本更新后名称和位置可能变化。未实际配置密钥或测试调用。来源：[[raw/2026-11-14-DeepSeek Harness 接入 TokenAge 简明教程]]

## 待核验

- [ ] 不同 OS 版本和 Harness 版本下的界面路径一致性。
- [ ] TokenAge 模型 `gpt-6.1-terra` 的实际可用性和定价。
