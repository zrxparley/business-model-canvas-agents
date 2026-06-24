# Command Manual

> **One unified entry `/bmc`, with keyword combinations for precise team activation.**

---

## Design Principle

```
[Action] + [Target] + [Business]
```

Example: `/bmc full-diagnosis AI resume optimization`

---

## 1. Unified Entry

### `/bmc`
All BMC team invocations use this prefix.

---

## 2. Core Commands (7)

### 1️⃣ `/bmc full-diagnosis`

**Trigger scenario**: Pre-launch check, quarterly review, pre-funding self-audit

**Template**:
```
/bmc full-diagnosis
Business: [name]
Customer: [who]
Value proposition: [one sentence]
Stage: [idea/MVP/growth/transformation]
Confusion: [Top 1-3 concerns]
Background: [team, revenue, key partnerships]
Output: [full 7-piece / key modules / priority optimization]
```

**Default team**: All 14 roles

**Expected time**: 1-2 hours

**Output**: 7-piece diagnostic report

---

### 2️⃣ `/bmc focused-diagnosis`

**Trigger scenario**: Quick breakthrough on a specific issue

**Template**:
```
/bmc focused-diagnosis [module-name]
Business: [name]
Problem: [specific issue]
```

**Example**:
```
/bmc focused-diagnosis CH
Business: AI resume optimization
Problem: CAC rose to 200, should we switch from Zhihu channel?
```

**Default team**: Target module expert + 2-3 upstream/downstream experts

**Expected time**: 20-30 minutes

---

### 3️⃣ `/bmc stress-test`

**Trigger scenario**: Quick validation of a new idea

**Template**:
```
/bmc stress-test
Idea: [description]
Target customer: [who]
Market: [where]
```

**Default team**: 3 feasibility experts only (no 9 module experts)

**Expected time**: 10-15 minutes

**Output**: Feasibility triangle score + one-line stress-test verdict

---

### 4️⃣ `/bmc customer-needs`

**Trigger scenario**: Want to understand "why customers really buy"

**Template**:
```
/bmc customer-needs
Business: [name]
Current VP: [current value proposition]
```

**Default team**: Customer Needs Expert + CS + VP

**Output**: JTBD task list + customer journey map + VP match score

---

### 5️⃣ `/bmc financial-checkup`

**Trigger scenario**: Cash flow, unit economics, growth flywheel issues

**Template**:
```
/bmc financial-checkup
Business: [name]
Current LTV: [number / don't know]
Current CAC: [number / don't know]
Current repurchase rate: [number / don't know]
```

**Default team**: Delivery Feasibility Expert + RS + CST + KA

**Output**: Unit economics model + cash flow health grade + flywheel diagram

---

### 6️⃣ `/bmc market-checkup`

**Trigger scenario**: Entering new market, choosing partners, evaluating competition

**Template**:
```
/bmc market-checkup
Business: [name]
Target market: [region / customer segment]
Partners: [candidate partners / don't know who]
```

**Default team**: Market Feasibility Expert + KP + CH

**Output**: Four-dimension radar + key dependency list + implementation path

---

### 7️⃣ `/bmc canvas`

**Trigger scenario**: Have conclusions, need visualization output

**Template**:
```
/bmc canvas [type]
Content: [conclusion description]
```

**Type options**:
- `bmc` — 9-cell BMC canvas
- `flywheel` — Growth flywheel diagram
- `journey` — Customer journey diagram
- `coherence` — Module coherence diagram
- `timeline` — Optimization path timeline

**Example**:
```
/bmc canvas bmc
Content: AI resume optimization subscription,
CS=30yo internet job seekers, VP=30s resume fix,
CH=Zhihu+Liepin, RS=monthly subscription, CST=AI compute
```

---

## 3. Shortcut Commands (10 high-frequency questions)

| Shortcut | Team Activated | Problem Solved |
|----------|----------------|----------------|
| `/bmc profitable` | Delivery Feasibility + RS + CST | Can the unit economics work? |
| `/bmc want-it` | Customer Needs + CS + VP | Do customers really want it? |
| `/bmc enter-market` | Market Feasibility + KP + CH | Market timing & ecosystem |
| `/bmc switch-channel` | CH + CR + KP | Channel ROI evaluation |
| `/bmc raise-price` | RS + Customer Needs + VP | Price increase feasibility |
| `/bmc boost-retention` | CR + Customer Needs + RS | Repurchase bottleneck |
| `/bmc cut-cac` | CH + KA + Customer Needs | Customer acquisition cost |
| `/bmc flywheel` | Delivery Feasibility + KA + CR | Growth flywheel |
| `/bmc coherence` | Coherence Auditor | Module consistency |
| `/bmc quarterly` | All 14 roles | Quarterly strategy review |

---

## 4. Contextual Commands

### `/bmc compare`
**Trigger scenario**: Compare two business models / two versions

**Template**:
```
/bmc compare
A: [business 1 description]
B: [business 2 description]
Dimension: [full / financial only / customer only / market only]
```

---

### `/bmc retrospective`
**Trigger scenario**: Previous diagnosis exists, want to see evolution

**Template**:
```
/bmc retrospective [previous diagnosis date]
Business: [name]
This quarter changes: [key changes]
```

---

### `/bmc industry [name]`
**Trigger scenario**: Diagnose within a specific industry (injects industry knowledge)

**Template**:
```
/bmc industry [industry-name]
Task: [diagnosis request]
```

**Supported industry keywords**:
- `SaaS` / `ecommerce` / `content` / `education` / `healthcare` / `fintech` / `local-services` / `hardware` / `cross-border` / `B2B` / `B2C` / `platform`

---

## 5. Quick Reference

```
📋 Core Commands (7)
  /bmc full-diagnosis        → Full team deep check
  /bmc focused-diagnosis     → Lock onto single module
  /bmc stress-test           → Quick new idea validation
  /bmc customer-needs        → JTBD customer insight
  /bmc financial-checkup     → Unit economics + flywheel
  /bmc market-checkup        → Timing + ecosystem + competition
  /bmc canvas                → mermaid visualization

📋 Shortcut Commands (10)
  /bmc profitable        /bmc want-it        /bmc enter-market
  /bmc switch-channel    /bmc raise-price    /bmc boost-retention
  /bmc cut-cac           /bmc flywheel       /bmc coherence
  /bmc quarterly

📋 Contextual Commands (3)
  /bmc compare              → A vs B model comparison
  /bmc retrospective        → Cross-quarter evolution analysis
  /bmc industry [name]      → Inject industry knowledge
```

---

## 6. Usage Examples (Copy-Paste Ready)

### Full Diagnosis
```
/bmc full-diagnosis
Business: AI Resume Optimization Service
Customer: 30-under job-seeking internet workers
Value proposition: 30-second resume makeover to FAANG standard
Stage: MVP, monthly revenue 50K
Confusion: CAC up to 200, repurchase only 8%, afraid to raise price
Team: 3 people
Partners: Liepin, Zhihu
Output: full 7-piece
```

### Stress Test
```
/bmc stress-test
Idea: AI tutoring for elementary school kids
Customer: dual-income families in tier-1 cities, grades 1-3
Market: 100M+ elementary students in China
```

### Shortcut Command
```
/bmc profitable
Business: AI writing tool with membership
Current LTV: 120
Current CAC: 80
Current repurchase rate: 45%
```

### Industry Injection
```
/bmc industry SaaS
full-diagnosis
Business: Project management SaaS
...
```

### Canvas Output
```
/bmc canvas flywheel
Business: AI resume optimization
Content: user growth → data optimization → experience improvement → repurchase → user growth
```

---

## 7. Command Combos

**Advanced usage**: Combine multiple commands to construct complex tasks

### Combo 1 · Stress Test + Full Diagnosis
```
/bmc stress-test AI legal consultation tool
(if verdict is "worth doing")
→ /bmc full-diagnosis
Business: AI legal consultation tool
...
```

### Combo 2 · Multiple Focused Diagnoses
```
/bmc customer-needs
Business: XX product
(after JTBD output)
→ /bmc focused-diagnosis VP
Business: XX product
Task: Rewrite value proposition based on JTBD
```

### Combo 3 · Compare + Canvas
```
/bmc compare
A: membership vs B: pay-per-use
(after comparison conclusion)
→ /bmc canvas flywheel
Content: membership flywheel
```

---

## 8. Top 3 Most-Used Commands

If you only remember 3:

1. **`/bmc full-diagnosis`** — Comprehensive health check
2. **`/bmc stress-test`** — Idea validation
3. **`/bmc customer-needs`** — Customer insight

**These 3 cover 80% of use cases.**

---

## 📖 Other Languages

- [中文版 (Chinese)](./commands.zh-CN.md)
