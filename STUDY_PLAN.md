# Claude Certification Study Plan: 4 Exams, 2 Weeks Apart

Order: **Associate → Developer → Architect Foundations → Architect Professional**, all taken online with Pearson VUE OnVUE.

> Exam facts below come from third-party prep sites (as of Oct 2026), not Anthropic's own pages. Before booking, confirm codes, fees, domain weights and eligibility in the **official exam guide** for each exam (Anthropic Partner Academy, or the Anthropic page on Pearson VUE).

## The four exams at a glance

| # | Exam | Code | What it tests | Reported domains |
|---|------|------|---------------|------------------|
| 1 | Claude Certified Associate – Foundations | CCAO-F | Using Claude well at work: prompting, product/model choice, evaluating output, responsible use | 7 |
| 2 | Claude Certified Developer – Foundations | CCDV-F | Building on the Claude API: apps, tools/MCP, model selection, prompt and context engineering, security, evals | 8 |
| 3 | Claude Certified Architect – Foundations | CCAR-F (also called CCA-F) | Designing agentic systems: orchestration, Claude Code, MCP, structured output, context and reliability | 5 |
| 4 | Claude Certified Architect – Professional | CCAR-P | Everything in CCAR-F, plus enterprise integration, governance and risk, stakeholders, lifecycle, developer enablement | 7 |

Common format (reported): about 120 minutes, scaled score with **720** to pass, proctored online (OnVUE) or at a test center, roughly $99–$175 per exam. Delivery moved to Pearson VUE on 30 Jun 2026, and the official practice exam was retired then.

### Reported domain weights

**CCAR-F (Architect Foundations).** Sources agree on these weights.
- Agentic architecture & orchestration: 27%
- Claude Code configuration & workflows: 20%
- Prompt engineering & structured output: 20%
- Tool design & MCP integration: 18%
- Context management & reliability: 15%

**CCAO-F (Associate).**
- Output evaluation & validation: 21%
- Workflow integration & solution design: 16%
- Governance, risk & responsible use: 15%
- Prompting & task execution: 14%
- Product & model selection: 12%
- Configuration & knowledge management: 12%
- Troubleshooting & optimization: 10%

**CCDV-F (Developer).** Sources agree on the 8 domain names but not on their weights: Applications & integration, Model selection & optimization, Agents & workflows, Prompt & context engineering, Tools & MCP, Security & safety, Claude Code, Eval/testing/debugging. Treat *applications/integration* as the heaviest.

**CCAR-P (Architect Professional).** 7 domains. Integration is reported as the heaviest at about 19%. Topics not in the Foundations exams: governance & risk, stakeholder communication & lifecycle, developer enablement.

---

## Why this order works

Each exam builds on the one before it, so most of what you study carries forward:

```
Associate (use Claude) ──► Developer (build with the API) ──► Architect F (design agents) ──► Architect P (run it in an enterprise)
     prompting, eval            + tools, MCP, SDKs              + orchestration, Claude Code     + governance, integration,
     model choice               + security, testing             + context & reliability          stakeholders, enablement
```

---

## Proposed calendar (starting Sat 31 Oct 2026)

| Window | Focus | Exam day |
|--------|-------|----------|
| 31 Oct – 13 Nov | CCAO-F | **Sat 14 Nov** |
| 15 Nov – 27 Nov | CCDV-F | **Sat 28 Nov** |
| 29 Nov – 11 Dec | CCAR-F | **Sat 12 Dec** |
| 13 Dec – 25 Dec | CCAR-P | **Sat 26 Dec** (or move to early Jan around the holidays) |

Book all four slots now. OnVUE slots fill up, and fixed dates keep the pace honest. Pearson lets you reschedule if you do it more than 24 hours before the exam; check the current policy when you book.

---

## The 2-week cycle (repeat for each exam)

Plan for about 2 hours on weekdays and 4–5 hours on weekend days, roughly 25–30 hours per exam.

**Days 1–2: Map the exam.**
Read the official exam guide line by line and turn every task statement into a checklist. Rate yourself 0–3 on each one.

**Days 3–8: Learn and build (most of your time).**
Spend this on the weakest, heaviest-weighted domains first. Use Anthropic Academy / Skilljar courses and the docs at docs.claude.com. *Build something* every day, because these exams are scenario-based and test judgment, not definitions.

**Days 9–11: Practice under exam conditions.**
Do timed scenario questions. For every miss, write down *why* the right answer is better, not just what it is. Questions often have 2 plausible options, and the best one is usually the simplest, safest or most reliable.

**Days 12–13: Close gaps and review lightly.**
Re-do the weak items on your checklist and re-read your notes of mistakes. Do the OnVUE system test (see below). Stop heavy study the evening before.

**Day 14: Exam.**

---

## Per-exam study focus

### 1. CCAO-F (Associate)
- **Prompting:** clear instructions, examples (few-shot), XML tags, giving Claude a role, letting it think step by step, prompt chaining.
- **Choosing the model and product:** Opus vs Sonnet vs Haiku (trade-offs between capability, speed and cost); Claude.ai vs Claude Code vs the API; Projects, Artifacts, connectors, Skills.
- **Evaluating output (heaviest domain):** spotting hallucinations, verifying against sources, asking for citations, writing rubrics.
- **Governance:** data handling, human review, avoiding misuse, admin controls.
- **Hands-on:** do a week of your real work through Claude.ai Projects with custom instructions and knowledge files.

### 2. CCDV-F (Developer)
- **Messages API:** roles, system prompts, `max_tokens`, `stop_reason`, streaming, handling errors and retries, rate limits.
- **Tool use:** JSON schemas, the tool loop, `tool_choice`, running tools in parallel, returning tool errors.
- **Structured output:** making Claude return valid JSON reliably; validating it and retrying.
- **Cost and performance:** prompt caching, the Batch API, counting tokens, choosing the model, extended thinking.
- **MCP:** servers, clients, tools, resources and prompts; local vs remote transports.
- **Security:** prompt injection, least privilege, keeping secrets out of prompts, filtering output.
- **Evals:** test sets, LLM-as-judge, regression testing for prompts.
- **Hands-on:** build a small Python or TypeScript app that uses tools, streaming, caching and a JSON-validated output, plus one MCP server.

### 3. CCAR-F (Architect Foundations)
- **Agentic architecture (27%):** workflows vs agents; patterns such as routing, parallelization, orchestrator-workers and evaluator-optimizer; when *not* to use an agent; subagents; the Claude Agent SDK.
- **Claude Code (20%):** CLAUDE.md hierarchy, settings and permissions, hooks, slash commands, Skills, subagents, MCP configuration, headless use in CI.
- **Prompting and structured output (20%):** designing schemas, few-shot prompting, extraction pipelines.
- **Tools and MCP (18%):** tool granularity and naming, descriptions, error contracts, choosing an MCP server vs a direct tool.
- **Context and reliability (15%):** managing the context window, compaction, memory, retrieval, idempotency, handing off to a human, recovering from failures.
- **Hands-on:** configure Claude Code on a real repo (CLAUDE.md, a hook, a custom subagent, an MCP server), then build a multi-step agent with the Agent SDK.

### 4. CCAR-P (Architect Professional)
- Everything in CCAR-F, at greater depth and with more trade-offs.
- **Enterprise integration (heaviest):** identity and SSO, data residency, cloud platforms (Bedrock, Vertex AI), gateways, observability.
- **Governance and risk:** policy, audit trails, evaluation gates, red-teaming, compliance.
- **Stakeholders and lifecycle:** writing the business case, ROI, rollout plans, change management, rolling back after a regression.
- **Developer enablement:** shared prompt and tool libraries, platform standards, internal training.
- **Hands-on:** write 2–3 one-page architecture decision records for realistic enterprise scenarios, such as a support agent, a document pipeline and coding-agent rollout across an org.

---

## Pearson OnVUE checklist (online proctored)

- [ ] Run the **OnVUE system test** on the *same* computer and network you'll use on exam day. Do it once a few days before and again the day before.
- [ ] Use a personal machine if you can; work laptops with VPNs or security agents often fail. Wired internet is best.
- [ ] Have a valid, unexpired government photo ID whose name exactly matches your Pearson profile.
- [ ] Clear your desk and walls of notes, papers and second monitors (unplug them). Keep your phone out of reach once check-in is done.
- [ ] Use a quiet, private room where nobody else can enter.
- [ ] Start check-in **30 minutes early**. You'll photograph your room and ID, and late arrivals can be refused.
- [ ] Stay in view of the camera. Don't read questions aloud or cover your mouth, and only take breaks if the rules allow.

---

## Primary resources

- Each exam's official **exam guide**, from Anthropic Partner Academy or the Anthropic page on Pearson VUE. This is your syllabus.
- **Anthropic Academy** (anthropic.skilljar.com): courses on the Claude API, MCP, Claude Code, agent skills and AI fluency.
- **Docs:** docs.claude.com (API, tool use, prompt engineering, prompt caching, Agent SDK), code.claude.com/docs (Claude Code), modelcontextprotocol.io.
- **Anthropic engineering posts:** *Building effective agents*, *Effective context engineering for AI agents*, *Writing tools for agents*.
- **anthropics/courses** and **anthropics/claude-cookbooks** on GitHub, for hands-on notebooks.

## Progress tracker

| Exam | Booked | Guide checklist done | Practice ≥ 80% | Passed |
|------|--------|----------------------|----------------|--------|
| CCAO-F | [ ] | [ ] | [ ] | [ ] |
| CCDV-F | [ ] | [ ] | [ ] | [ ] |
| CCAR-F | [ ] | [ ] | [ ] | [ ] |
| CCAR-P | [ ] | [ ] | [ ] | [ ] |
