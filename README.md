# KayingCodex

**面向 HarmonyOS 应用开发的 AI 驱动桌面工作台。**

把通用 Coding Agent 能力，收束成真正适合 HarmonyOS 开发流程的桌面产品。

---

## 简介

KayingCodex 是一款桌面端 AI 开发产品，基于 OpenCode 能力构建，并针对 HarmonyOS 开发场景做了明确强化。

它不是泛用聊天壳，也不是普通代码补全插件，而是一个围绕 **HarmonyOS 项目工作区、ArkTS / ArkUI 规则、构建部署、自动化流水线、工作树隔离、代码审查与语料沉淀** 组织起来的 AI 工作台。

---

## HarmonyOS 专属能力

| 模块 | 说明 |
|---|---|
| **Harmony Scaffold** | Stage 项目创建、SDK 路径检测、模块结构校验 |
| **ArkUI Patterns** | 布局、状态管理、导航与动画最佳实践技能 |
| **ArkTS Rules** | 类型约束识别、编译问题诊断、禁用特性检测 |
| **Build & Debug** | hvigorw 构建、hdc 部署、hilog 日志分析与常见错误修复 |
| **Abilities** | UIAbility 生命周期、路由管理、权限声明与申请流程 |
| **Pipeline** | 七阶段自动化流水线：分析 → 脚手架 → 开发 → 编译 → 修复 → 校验 → 报告 |

支持 HarmonyOS NEXT API 12+、ArkTS、ArkUI、Stage Model、hvigorw、hdc、ohpm。

---

## 桌面产品能力

- **多项目工作区** — 独立管理多个 HarmonyOS 项目，每个工作区拥有独立会话与工具链配置
- **Review Panel** — 文件差异可视化与评论，在接受 Agent 改动前清楚查看每一处变更
- **Worktree 隔离** — 在隔离的 Git 工作树中执行 Agent 任务，保护主工作区，随时回滚
- **Automations** — 定时任务与自动化规则，把高频重复操作从手动触发变为可调度执行
- **Corpus 语料** — 从开发会话中采集有效语料，支持多格式导出，用于微调或团队知识库沉淀
- **子 Agent 权限** — 子 Agent 权限上浮机制，可控的工程助手，不是黑盒改代码

---

## 工程工作流

```
添加项目 / 进入工作区
        ↓
用自然语言描述需求
        ↓
Agent 结合 HarmonyOS 技能生成 / 修改代码
        ↓
hvigorw 构建与修复循环
        ↓
Review Panel 审查改动
        ↓
Worktree 隔离执行（可选）
        ↓
沉淀到 Pipeline / Corpus / Automations
```

---

## 安装

从 GitHub Releases 下载适合你平台的安装包：

**[→ 查看 Releases](https://github.com/kaying-studio/kaying-codex/releases)**

| 平台 | 格式 |
|---|---|
| macOS | `.dmg` / `.zip` |
| Windows | NSIS 安装包 / Portable |
| Linux | `.AppImage` / `.deb` / `.rpm` |

> 需要自行配置模型 Provider 和对应的 API Key（支持 Anthropic、OpenAI 兼容接口及本地模型）。

---

## 免费使用

KayingCodex 免费提供下载与使用，持续迭代更新中。

---

## 更多信息

官网：**[https://kaying.studio](https://kaying.studio)**

---

*KayingCodex 由 [KaYing Studio](https://kaying.studio) 开发与维护。*
