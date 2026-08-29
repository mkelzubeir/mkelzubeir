## About Me

# Mohammed Elzubeir

**Builder-operator.** New York City. *Open to new roles.*

Across my roles, I’ve been responsible for making quality concrete. At McMaster-Carr, I led a 12-person operations team while defining performance standards. At OpenAI, I tested where frontier models broke down. More recently, I founded a company building expert-led evaluations for medical AI.

---

## Projects

### [atlas-industrial-ai](https://github.com/mkelzubeir/atlas-industrial-ai) — industrial-distribution voice agent

A voice agent for a synthetic industrial distributor, informed by workflows I managed in industrial customer-service operations. In one spoken conversation, a caller can check an order or shipment, resolve an ambiguous product description, verify inventory, request a quote, and modify an eligible order line. The ElevenLabs agent manages the conversation and selects tools; seven FastAPI webhook APIs remain authoritative about business data and permitted actions.

Business rules are enforced server-side, including explicit confirmation for writes, line-level edit eligibility, and inventory constraints. Successful and rejected changes are audited, RFQ creation is idempotent, and optimistic concurrency prevents stale order updates. A Next.js Developer View exposes tool arguments, responses, and state changes during each call. The repository includes 132 passing pytest tests and 12 conversational evaluation scenarios covering hallucinated facts, premature writes, ambiguous products, tool failures, and dropped intents. All customers, products, orders, and operational rules are synthetic. [Live app](https://atlas-industrial-ai.vercel.app/).

### [ai-interviewer](https://github.com/mkelzubeir/ai-interviewer) — voice-first AI mock interviewer

Upload a resume and job description, then sit a real spoken interview: an AI interviewer that asks questions grounded in your actual background and the role, listens over live speech-to-speech (OpenAI Realtime over WebRTC), handles interruptions and turn-taking with server-side voice activity detection, and probes with follow-ups the way a human interviewer would. Every session ends in a structured feedback report.

Static site on GitHub Pages with exactly one server-side step, minting ephemeral Realtime tokens, pushed into a JWT-verified, rate-limited Supabase Edge Function so the permanent API key never ships to a browser. Local-first by default: in-progress sessions live in localStorage and the deterministic question engine runs entirely client-side, with optional sign-in to persist reports behind row-level security. 120+ unit tests and a Playwright suite that runs against the production static build in CI, so subpath and fallback bugs get caught before deploy. [Live app](https://mkelzubeir.github.io/ai-interviewer/).

### [logic-console](https://github.com/mkelzubeir/logic-console) — clinical red-teaming platform
Trauma surgeons capture gold-standard management plans for clinical scenarios, then blind-grade frontier model outputs against them using span-level severity classification (acceptable / harmful / lethal) with structured rationales, plus a transcript-level omission check — because a commission-only model can't catch dangerous absences.

Designed and shipped solo, deployed to production annotators. Supabase/Postgres with row-level security across all clinical tables, closed-registration auth with annotator identity derived from verified JWTs, and provenance controls throughout (immutable snapshots, dated model version strings). Includes an evaluation harness for generating comparison data across models.

Built at Insaan, a company I founded. All case data in the repo is synthetic.

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
