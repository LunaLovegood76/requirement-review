# 需求评审模拟器 | Requirement Review Simulator

<details>
<summary>🌐 Read in English</summary>

### Introduction

A Claude Skill for product managers that simulates real-world requirement review meetings. Compatible with **Claude Code, OpenClaw**, and other agent platforms that support the Claude Skill protocol. By roleplaying as **Tech Lead, UX Designer, QA Engineer, and Business Stakeholder**, it helps you discover blind spots in your PRD, fill in edge cases, and strengthen your arguments — all before the actual review meeting.

> Inspired by the most common pain points in product requirement reviews: getting challenged by engineers, missing edge cases, vague acceptance criteria, and rubber-stamp reviews that catch nothing.

### Features

- **PRD Health Scan** — Auto-detects gaps across 9 dimensions with a visual dashboard
- **4-Role Simulation** — Each role has a distinct persona and communication style
- **Interactive Q&A** — One question at a time, with feedback after each answer
- **Structured Review Report** — Problem list, action items, and pre-meeting tips
- **3 Review Modes** — Full review (10-15 questions) / Quick review (4 questions) / Single role

### Installation

**Claude Code**
```bash
# Global install (available in all projects)
~/.claude/skills/requirement-review/SKILL.md

# Project-level install (current project only)
your-project/.claude/skills/requirement-review/SKILL.md
```

**OpenClaw & other platforms**

Refer to your platform's documentation for the Skill directory path. The skill file has no platform-specific dependencies and should work with any agent tool that supports the Claude Skill protocol.

### Usage

```bash
# Start an interactive review session
/requirement-review

# Directly review a PRD file
/requirement-review ~/Desktop/my-prd.md
```

### Review Workflow

```
Phase 0  Input          → File path / Direct description / Paste content
Phase 1  Understanding  → Summarize core requirements, confirm alignment
Phase 2  Health Scan    → 9-dimension check + visual dashboard
Phase 3  Role Reviews   → Tech → Design → QA → Business (one question at a time)
Phase 4  Report         → Problem list + action items + pass/fail recommendation
Phase 5  Wrap-up        → Save report / Deep dive / Re-review
```

### The Four Review Roles

| Role | Persona | Focus Areas |
|------|---------|-------------|
| 🔧 Tech Lead | 8yr backend, pragmatic | Feasibility, data sources, error handling, API definitions |
| 🎨 UX Designer | 5yr UX, zero tolerance for ambiguity | Empty states, loading feedback, user flows, multi-platform |
| 🔍 QA Engineer | 6yr testing, born to find bugs | Acceptance criteria, edge cases, regression scope, data consistency |
| 💼 Business Stakeholder | Product director, ROI-focused | Business value, data evidence, competitive analysis, measurability |

### Requirements

- Any agent platform that supports the Claude Skill protocol (Claude Code, OpenClaw, etc.)
- No external tools or MCP servers required

### License

MIT

</details>

---

## 简介

一个为产品经理设计的 Claude Skill，可用于 **Claude Code、OpenClaw** 等支持 Claude Skill 协议的 Agent 平台。通过模拟真实互联网公司的需求评审会议，扮演**技术负责人、交互设计师、测试工程师、业务方**四个角色，帮助你在正式评审前发现 PRD 盲区、补齐边界条件、强化需求论据。

> 灵感来源：产品经理在需求评审中最常见的痛点——被开发怼、边界遗漏、验收标准模糊、评审走过场。

## 功能特性

- **PRD 健康度扫描** — 9 个维度自动检测，可视化仪表盘展示薄弱环节
- **四角色模拟评审** — 每个角色有独立人设和语气，模拟真实评审氛围
- **交互式问答** — 每次只抛一个问题，等你回答后给出反馈再继续
- **结构化评审报告** — 包含问题清单、行动项、上会 Tips
- **三种评审模式** — 完整评审（10-15问）/ 快速评审（4问）/ 指定角色

## 安装

将 `SKILL.md` 放到对应平台的 Skill 目录：

**Claude Code**
```bash
# 全局安装（所有项目可用）
~/.claude/skills/requirement-review/SKILL.md

# 项目级安装（仅当前项目可用）
你的项目/.claude/skills/requirement-review/SKILL.md
```

**OpenClaw 及其他平台**

参考各平台文档，将 `SKILL.md` 放入对应的 Skill 加载目录即可。Skill 文件本身不依赖平台特定功能，理论上兼容所有支持 Claude Skill 协议的 Agent 工具。

## 使用方式

```bash
# 启动评审（交互式选择需求输入方式）
/requirement-review

# 直接指定 PRD 文件路径
/requirement-review ~/Desktop/my-prd.md
```

## 评审流程

```
Phase 0  需求输入       → 文件路径 / 直接描述 / 粘贴内容
Phase 1  需求理解确认   → 复述核心，确认理解一致
Phase 2  PRD健康度扫描  → 9维检查 + 可视化仪表盘
Phase 3  四角色评审     → 技术 → 设计 → 测试 → 业务（逐一交互）
Phase 4  评审报告       → 问题清单 + 行动项 + 通过建议
Phase 5  收尾           → 保存报告 / 深入讨论 / 重新评审
```

## 四个评审角色

| 角色 | 人设 | 关注点 |
|------|------|--------|
| 🔧 技术负责人 | 8年后端经验，务实不刻薄 | 技术可行性、数据来源、异常处理、接口定义 |
| 🎨 交互设计师 | 5年UX经验，对模糊零容忍 | 空状态、加载反馈、操作路径、多端适配 |
| 🔍 测试工程师 | 6年QA经验，天职是找bug | 验收标准、边界条件、回归范围、数据一致性 |
| 💼 业务方/老板 | 产品总监，关心ROI | 需求价值、数据支撑、竞品对比、可度量性 |

## 系统要求

- 支持 Claude Skill 协议的 Agent 平台（Claude Code、OpenClaw 等）
- 不依赖任何外部工具或 MCP
