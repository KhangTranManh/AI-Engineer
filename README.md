# 📄 Tran Manh Khang – CV

**AI Engineer — LLM, AI Agents & Model Evaluation**

📧 khangjaki12@gmail.com · 📍 My Tho, Tien Giang, Vietnam · 🐙 [github.com/KhangTranManh](https://github.com/KhangTranManh)

Welcome to my CV repository! This repo holds my up-to-date CV and a quick overview of my experience, projects and skills.

---

## 👋 About Me

Final-year Software Engineering student focused on **making LLM systems measurably reliable**.

- Built and fine-tuned an LLM workflow for customer-call quality assessment at **Concentrix**.
- Ran a **10-phase independent study** on whether a small LLM can catch its own mistakes, using automatic answer checking instead of an AI judge.
- Comfortable turning failures into controlled experiments, reporting negative results honestly, and building agents with safety guardrails.

---

## 📂 Selected Projects

### 🔬 LLM Self-Correction Research
*Personal research project · 10 phases*

**Problem:** can a small language model detect and fix its own wrong answers?

- **Evaluation without an AI judge:** math answers checked symbolically and code run against tests; all test sets frozen and kept separate from training data.
- **Voting works:** majority vote over 5 independent attempts raised GSM8K accuracy from **75.0% → 83.25–85.5%** on 400 fresh problems across three model versions (p < 0.001).
- **Knows *that*, not *which*:** disagreement between two attempts caught **82–85%** of wrong first answers, but the model picked the right one of two conflicting solutions only **44–52%** of the time.
- **Fixes that failed, reported as such:** a fine-tuned judge (808 balanced examples) stayed at chance (52.1% → 50.7%) and trailed voting by 6 points; preference tuning raised KEEP recall 81% → 85% without better error detection.
- **Blind re-solve helps:** a second attempt that does not see the earlier answer fixed far more errors; routing flagged answers to it lifted accuracy from **70.75% → 74.5–77.5%**.
- All data, configs and evaluation code kept reproducible.

### 🤖 Ciel — Personal AI Agent
*Personal project · Python, Docker*

**Problem:** let an LLM plan and act with real tools without unsafe or duplicate actions.

- **Brain/Worker design:** one model classifies intent and plans, another responds; deterministic code validates plans, permissions, budgets and cancellation — *the model proposes, the code enforces*.
- **Guardrails:** malformed multi-tool plans stop before execution, risky actions need confirmation, file access is sandboxed, and outgoing messages and reminders are deduplicated across restarts.
- **Product features:** monthly/weekly planning, one-time reminders, long-term memory (ChromaDB) and proactive Telegram notifications on one runtime shared by CLI, API/web UI and Telegram; deployed with Docker.
- **Prompt-improvement tool:** mines repeated failures and may edit only one allow-listed prompt string; auto-reverts if unit tests fail. Backed by a regression test suite.

---

## 💼 Experience

### AI Engineer Intern — Concentrix, Vietnam
*Mar 2026 – Jul 2026*

- Built an LLM-based workflow to assess customer-call quality: converted conversations into structured data and validated predictions against human-labeled samples.
- Fine-tuned a small open-source LLM, focusing training on hard cases where earlier versions failed, which substantially improved accuracy.
- Benchmarked it against leading commercial models: comparable on straightforward cases, stronger on difficult ones, at a lower inference cost.
- Tested AI agent workflows for reliability: retry/fallback behavior, tool-response validation, edge-case documentation and prompt improvements.

### Exchange Student Program — JeonJu University, Korea
*2024*

- Studied AI, Machine Learning and Deep Learning as an exchange student.

---

## 🎓 Education

**B.Eng. Software Engineering — Ton Duc Thang University** *(2021 – 2026)*
IELTS 6.0

---

## 🛠 Skills

| Area | Tools & Techniques |
|---|---|
| **LLM & ML** | PyTorch, Unsloth, fine-tuning (SFT, DPO, GRPO, ORPO), model evaluation, representation probing, activation steering |
| **Agent systems** | LangChain, LangGraph, tool calling, retry/fallback workflows, guardrails, ChromaDB (RAG) |
| **Computer vision** | YOLOv8, OpenCV |
| **Software & backend** | Python, Java, JavaScript, TypeScript, Node.js, Express, REST APIs, MongoDB, Docker, vLLM, Git |

---

## 📄 CV

[Download my latest CV (PDF)](./Tran_Manh_Khang_CV.pdf)

---

⭐ If you're interested in my work, feel free to connect with me or check out my projects here on GitHub!
