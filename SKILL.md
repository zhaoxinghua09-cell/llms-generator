---
name: llms-generator
description: "Generate llms.txt (LLMs.txt v2 spec) and AI-discoverability packages for any project, so AI agents can find and read your assets. 为任意项目生成 llms.txt（LLMs.txt v2 规范）与 AI 可发现性包，让 AI 代理能找到并读懂你的资产。"
version: 1.0.0
license: MIT
category: 效率
author: SynomosAI (LGD initiative)
platforms: [windows, macos, linux]
tags: [llms-generator,ai-discoverability,llms-txt,seo]
slug: llms-generator
risk_tier: medium
---

# LLMs.txt Generator (AI 可发现性生成器)

> **One command to become AI-discoverable: llms.txt + ecosystem links.**
> **一条命令让项目被 AI 发现：llms.txt + 生态互链。**
> 理论根基：LGD 三律（有籍·有证·有门禁）· AEO（Agentic Engine Optimization）

## 背景 / Why
AI 代理通过 llms.txt / AGENTS.md 发现项目。没有 llms.txt 的项目对 AI 是"半盲的"。本技能一条命令生成规范文件。

## 功能 / Capabilities
- Generates llms.txt per LLMs.txt v2 spec (H1 title + curated links)
- Embeds ecosystem links (awesome/ORCID/Zenodo/SWH/standards) for AI agents
- Optionally inlines full markdown as llms-full.txt content
- 按 LLMs.txt v2 规范生成 llms.txt（H1 标题 + 精选链接）
- 内置生态互链（awesome/ORCID/Zenodo/SWH/标准）供 AI 代理读取
- 可选内联全文作为 llms-full 内容

## 用法 / Usage
```bash
python scripts/llms_gen.py --name MyProject --url https://github.com/org/repo --desc "..." [--link ...] [--full README.md]
```

## 三律对齐 / LGD alignment
| 律 | 本技能如何满足 |
|---|---|
| 有籍 Registered | 输出带项目名/URL/作者 ORCID，身份明确 |
| 有证 Evidenced | 生成内容可复现，含生态互链证据 |
| 有门禁 Gated | 只生成文件不自动发布；覆盖时提示 |

## Standard alignment / 标准对齐
- **Agent Skills open standard**: compatible with [agentskills.io](https://agentskills.io) format (SKILL.md + scripts/, frontmatter name/description). Adopted by Claude/Codex and the broader agent ecosystem.
- **AEO**: llms.txt / AGENTS.md friendly (AI-agent discoverable).

## Skill card / 技能卡（对标 NVIDIA Verified Agent Skills）
- **Ownership / 所有权**: SynomosAI initiative — Steven Zhao (ORCID 0009-0001-0512-1237)
- **Dependencies / 依赖**: none (Python 3 stdlib only)
- **Limitations / 限制**: static analysis only; not a substitute for runtime verification
- **Verification status / 验证状态**: self-reported PASS via skill-quality-gate; not a certification or endorsement
- **Security posture / 安全姿态**: no network calls, no destructive operations, fail-closed exit codes

## License & attribution
**分层许可**：代码 `scripts/*.py` MIT；本 SKILL.md/README 及理论文本 All rights reserved。

```
© 2026 赵兴华 / Steven Zhao·China (ORCID 0009-0001-0512-1237). All rights reserved.
理论署名 (attribution) : LGD（Lifecycle Governance Doctrine / 全程治理论）— SynomosAI initiative
名称状态 (name status)  : "SynomosAI" / "MedXpert" — 未申请实体注册、未申请商标注册
生产参考部署 (production reference, self-reported) : MedXpert（非认证、非背书、非监管认可）
引用格式 (cite as)      : 本资产无 DOI
```
（《LGD 对外表述规范》§3.2 统一块，整体复制、未删改。）
