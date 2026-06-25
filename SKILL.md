---
name: intelligence-brain
slug: intelligence-brain
version: 1.0.0
displayName: Intelligence Brain
description: AI-native company intelligence engine with 8-step metabolic pipeline, cross-file inference, neural chain design, and information classification routing.
tags: [intelligence, knowledge-management, data-pipeline, agent-brain, information-classification, neural-chain]
license: MIT
---

# Intelligence Brain — AI-Native Company Intelligence Engine

Not a database. An engine.

Existing "brain" skills store facts. They cache. They retrieve. That's useful — but it's a library, not a brain. A real brain doesn't just store information. It ingests, digests, connects, infers, and outputs actionable intelligence.

Intelligence Brain is the engine that powered a live 7-department AI company's DataCenter — the department that gathered intelligence, managed agents, built neural chains, and produced cross-file inferences that no single document contained.

---

## What This Is

An intelligence processing methodology with concrete implementation patterns. The brain:

1. **Ingests** raw information from multiple sources
2. **Processes** it through an 8-step metabolic pipeline
3. **Infers** cross-document insights via WISDOM_GRAPH and ACTION_PIPELINE
4. **Routes** outputs based on information classification
5. **Manages** agent lifecycles and inter-agent neural chains

---

## The 8-Step Metabolic Pipeline

Raw information enters the company daily. Without a processing system, it accumulates as noise. The pipeline transforms noise into intelligence:

```
Step 1: READ     → Ingest incoming data (reports, research, outputs)
Step 2: PARSE    → Extract structured information from raw text
Step 3: DECOMPOSE→ Break into atomic facts, claims, and data points
Step 4: ORGANIZE → Categorize by domain, priority, and classification
Step 5: MERGE    → Cross-reference with existing knowledge, detect duplicates
Step 6: USE      → Apply to active decisions, content, or strategy
Step 7: DELETE   → Remove processed raw data (prevent accumulation rot)
Step 8: EXTRAPOLATE → Generate cross-file inferences (the "One More Thing" step)
```

**Time constraint**: All 8 steps must complete within 24 hours of ingestion. Unprocessed data decays in value exponentially.

### Step Detail: DECOMPOSE

```markdown
Input: "AI应用加速落地，2026年商业化提速，企业级应用增长300%"
Output:
  - [Claim] AI应用落地速度正在加快（来源：行业报告）
  - [Data] 企业级应用增长300%（需验证：来源、时间范围）
  - [Trend] 商业化从实验阶段进入加速阶段
  - [Action] 品牌部：可转化为"AI商业化"内容选题
```

### Step Detail: EXTRAPOLATE

The most valuable step. Cross-file inference finds insights that exist between documents, not within them:

```markdown
File A (品牌部报告): "小红书内容互动率下降15%"
File B (销售部报告): "知识星球付费转化率提升22%"

Cross-file inference: 免费平台引流效率下降 + 付费阵地转化上升
→ Action: 增加知识星球内容密度，减少小红书发布频率
→ Update: 变现漏斗权重调整
```

---

## Cross-File Inference System

### WISDOM_GRAPH

A network of insights connected across departmental outputs. Nodes are key findings. Edges are inferred relationships.

```
[小红书互动率↓] ──causes──→ [免费引流效率↓]
                                     │
                              ──suggests──→ [增加付费阵地投入]
                                     │
[知识星球转化↑] ──validates──→ [付费意愿存在]
```

### ACTION_PIPELINE

Inferences that become actionable tasks, prioritized by urgency:

| Priority | Count | Example |
|----------|-------|---------|
| P0 | ≤4 | AIGC标注合规、退款公示、广告合规、哈希锁定 |
| P1 | ≤4 | 内容策略调整、平台权重优化 |
| P2 | ≤4 | 工具升级、流程优化 |
| P3 | ≤4 | 长期研究、探索性项目 |

Max 4 items per priority tier. Forces ruthless prioritization.

### ONE_MORE_THING

The highest-value inference: insights that connect domains nobody else thought to connect. Example from production:

```
Marketing data + Legal compliance data → "平台政策变化将影响内容分发策略"
Sales data + Finance data → "客户获取成本上升但客单价未变 → 定价策略需调整"
```

---

## Neural Chain Architecture

The brain doesn't just process — it builds and maintains the communication infrastructure between agents.

### Design Principles

1. **Redundancy ≥ 3** — At least 3 parallel communication channels
2. **No single point of failure** — Any one channel can fail without breaking the system
3. **Async-first** — Agents read when ready, not when messaged
4. **Auditability** — Every inter-agent communication leaves a trace

### Chain Topology

```
         ┌──────────┐
         │   CEO    │ (Decision only)
         └────┬─────┘
              │
    ┌─────────┼─────────┐
    │         │         │
┌───▼──┐ ┌───▼──┐ ┌───▼──┐
│Brand │ │Sales │ │Legal │
└───┬──┘ └───┬──┘ └───┬──┘
    │         │         │
    └─────────┼─────────┘
              │
    ┌─────────▼─────────┐
    │    DataCenter     │ (Hub)
    └─────────┬─────────┘
              │
    ┌─────────┼─────────┐
    │         │         │
┌───▼──┐ ┌───▼──┐ ┌───▼──┐
│Financ│ │Insp. │ │Admin │
└──────┘ └──────┘ └──────┘
```

DataCenter is the hub, but NOT a bottleneck. Messages route through it, not queue at it.

---

## Information Classification & Model Routing

Every piece of information entering the brain gets classified, and classification determines which AI model processes it:

| Level | Label | Examples | Model Routing |
|-------|-------|----------|---------------|
| 🔴 TS | Top Secret | API keys, credentials, private tokens | Local only, never cloud |
| 🟠 C | Confidential | Financial data, strategy docs, user PII | Premium models (DeepSeek Pro) |
| 🟡 I | Internal | Dept outputs, reports, meeting notes | Free models (GLM-4-Flash) |
| 🟢 P | Public | Published content, marketing materials | Any model, any channel |

This is not just security — it's cost optimization. Why burn premium tokens on internal memos?

---

## Agent Lifecycle Management

The brain tracks every agent in the organization:

```
Agent: Brand Department
Status: ACTIVE
Cron Jobs: 3 (daily learning, daily report, content publish)
Last Activity: 2026-06-25 15:52 CST
Consecutive Errors: 0
Model: deepseek/deepseek-v4-pro (publish), zai/glm-4-flash (learning)
```

When an agent goes silent (no activity for 24h) or errors spike (2+ consecutive failures), the brain flags it for inspection.

---

## Implementation Guide

### Phase 1: Pipeline Setup
1. Establish the `company/data/` directory structure
2. Define data sources (department outputs, external feeds, research)
3. Implement the 8-step pipeline (initially manual, then cron-automated)
4. Set the 24h processing SLA

### Phase 2: Inference Engine
1. Build WISDOM_GRAPH from first week of processed data
2. Generate initial ACTION_PIPELINE
3. Validate inferences against real outcomes
4. Tune the extrapolation heuristics

### Phase 3: Neural Chain
1. Map existing communication paths
2. Identify single points of failure
3. Add redundant channels (minimum 3)
4. Test failure scenarios (kill one channel, verify others work)

---

## Dependencies

Designed for the **OpenClaw** agent runtime:
- `cron` for scheduled pipeline execution
- `sessions_send` for neural chain messaging
- Workspace file system for data persistence
- Multi-model routing for cost optimization

Methodology is platform-agnostic. Implementation details are OpenClaw-specific.

---

## Companion Skills

- **opc-os-core** — The complete one-person company operating system that this brain powers
- **agent-org-manager** — Multi-department setup and management
- **cron-health-monitor** — Cron job health monitoring (brain's self-diagnostic tool)

---

## License

MIT — Free to use, modify, distribute. Built from production intelligence operations, not theory.
