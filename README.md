## About Me

# Mohammed Elzubeir

**AI evaluation and operations.** New York City. *Open to new roles.*

I've worked both sides of the same problem: running operations teams against measurable quality standards, and testing whether AI systems hold up against them. I led a 12-person team at McMaster-Carr, red-teamed frontier models on contract for OpenAI, and founded a company building expert-governed evaluations for medical AI.

---

## Projects

### [logic-console](https://github.com/mkelzubeir/logic-console) — clinical red-teaming platform
Trauma surgeons capture gold-standard management plans for clinical scenarios, then blind-grade frontier model outputs against them using span-level severity classification (acceptable / harmful / lethal) with structured rationales, plus a transcript-level omission check — because a commission-only model can't catch dangerous absences.

Designed and shipped solo, deployed to production annotators. Supabase/Postgres with row-level security across all clinical tables, closed-registration auth with annotator identity derived from verified JWTs, and provenance controls throughout (immutable snapshots, dated model version strings). Includes an evaluation harness for generating comparison data across models.

Built at Insaan, a company I founded. All case data in the repo is synthetic.

<!-- ADD PROJECT 2 HERE -->

<!-- ADD PROJECT 3 HERE -->

---

## Background

**Insaan** — Founder. Recruited and managed senior trauma surgeons as expert annotators, owning onboarding, contractor agreements, cross-border data compliance, and consent for onward transfer to AI labs. Owned the red-teaming data pipeline end to end: adversarial scenario design, annotation workflows, and structured failure-mode capture.

**McMaster-Carr** — Strategy & Operations Lead. Promoted to supervisor within nine months. Led a team of 12 to the department's highest quality KPIs while cutting task completion time 15%. Partnered with engineering to translate contact-center workflows into API logic for an LLM copilot, mapping 100+ tasks into executable call sequences. Reset four-year-old performance benchmarks using distribution analysis in Python, landing targets 16% closer to observed capacity.

**OpenAI** - External Red Team Member (Contract). Conducted adversarial testing of large language and multimodal systems to surface failure modes and edge-case behaviors, contributing to risk assessments used in deployment decisions. Credited in the [GPT-4o system card](https://cdn.openai.com/gpt-4o-system-card.pdf) for contributions to AI safety strategy.


**Earlier** — Investment Analyst at Laurium Capital (hedge-fund), Product Management at Capital Group; Research Fellow at Harvard Business School

M.S. Information & Data Science, UC Berkeley 🐻 
A.B. Economics, Statistics and Machine Learning Certificate, Princeton 🐯

---

## How I work

Agentic coding tools are my primary development environment — logic-console was built and shipped this way, solo, including the schema design, auth model, and deploy pipeline. It lets me take a problem from spec to working system without waiting on an engineering queue.

**Areas:** LLM red teaming · expert annotation pipelines · harm taxonomies and quality rubrics · structured safety assessments · SQL (CTEs, window functions) · Python (Pandas, NumPy) · Supabase/Postgres · Tableau

---

## Contact

**mkfhelzubeir@gmail.com** · **[LinkedIn](https://www.linkedin.com/in/elzubeir/)**
<!--
**mkelzubeir/mkelzubeir** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
