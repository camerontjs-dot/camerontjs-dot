# Cameron Sanderson

I build and evaluate AI systems that have to survive review — agent evaluation harnesses, claim-support audits, and provenance pipelines.

The discipline comes from more than eight years in sterile pharma QA/QC (cGMP, USP &lt;797&gt;): preserve the source state, make failure modes testable, and leave enough evidence for someone else to challenge the result. That background is my credibility, not the only audience I write for.

Based in Ontario, Canada. Bilingual English and French.

## Start here (two paths, one minute)

### Path A — Claim support apparatus

1. [**Claim Audit Lab**](https://github.com/camerontjs-dot/claim-audit-lab) — audits whether draft claims are supported by *supplied* evidence (deterministic rules, Markdown + JSON reports, explicit limits).
2. [**Evidence Bundler**](https://github.com/camerontjs-dot/evidence-bundler) — nominates candidate passages into a reviewable bundle. Retrieval nominates; review decides.
3. [**Apparatus Contracts**](https://github.com/camerontjs-dot/apparatus-contracts) — versioned handoffs and integrity checks between those stages.

### Path B — Agent evaluation and completion honesty

1. [**agent-eval-notes**](https://camerontjs-dot.github.io/agent-eval-notes/) — public methods tour: harnesses that score better and are not promoted, multi-path coding screens, task-family transfer, RAG routes, verify-tool honesty.
2. [**verified-done**](https://github.com/camerontjs-dot/verified-done) — runnable demo: verified pass vs false completion vs scope violation, with a selftest and scrubbed live evidence.

Together, Path B treats **scope** and **false "done"** as first-class failures, not soft notes.

## How I know it works (two receipts)

- On a sealed coding-agent suite, a packet harness improved verified passes **28/36 → 34/36** and cleared scope violations **6 → 0**, then was **not promoted** because a pre-registered gate caught **2 false completion claims** on multi-file work (exploratory; details on the tour).
- On a public demo split, holding the model fixed and removing a `run_verify` tool flipped honesty outcomes (and a local open-weight coder reproduced the flip; another model already abstained either way). Method: [Report 06](https://camerontjs-dot.github.io/agent-eval-notes/report-06.html) + [verified-done](https://github.com/camerontjs-dot/verified-done).

Numbers are exploratory measurements with stated n, not production validation.

## Workspace and retrieval

- [**MainFrame**](https://github.com/camerontjs-dot/MainFrame) — public Stage 1b cut of a lifecycle-first Markdown knowledge OS (inbox → ingest → knowledge → live → projects → archive). Nested **MindGraph** local hybrid retrieval (lexical + semantic + graph). Private corpora stay private.
- [**MindGraph**](https://github.com/camerontjs-dot/MindGraph) — standalone package of the same engine when you only want the retriever.

## Other public work

- [**Career Decision Engine**](https://github.com/camerontjs-dot/career-decision-engine) — browser decision-support tool with visible scoring and confidence labels. [Live demo](https://camerontjs-dot.github.io/career-decision-engine/).
- [**Research Scaffold Harness**](https://github.com/camerontjs-dot/research-scaffold-harness) / [**Basic Research Harness**](https://github.com/camerontjs-dot/basic-research-harness) — scaffold and agent-loop experiments with provenance-oriented outputs.

## What this is not

These tools are not a truth engine, not a regulated quality system, and not a claim that production agents are “validated.” Evidence Bundler nominates. Claim Audit Lab audits relative to supplied evidence. Agent-eval numbers are sealed or demo-split measurements with stated limits. Software work is self-taught and project-based.

## What I am looking for

Work where AI systems meet review, reliability, and real operating constraints:

- AI evaluation, agent reliability, and evidence-handling workflows
- regulated software, quality systems, and data integrity
- forward-deployed or consulting work that maps a real process before automation

## Contact

- [LinkedIn](https://www.linkedin.com/in/cameron-sanderson/)
- [Email](mailto:camerontjs@gmail.com)
