# Cameron Sanderson

I build and evaluate AI systems around evidence, retrieval, agent behavior, and decisions under uncertainty.

My background is more than eight years in sterile pharmaceutical laboratory and quality work (cGMP, USP 797). The same habits carry into software: preserve source state, make failure modes testable, and leave enough evidence for someone else to challenge the result.

Based in Ontario, Canada. Bilingual English and French.

## Start here

### Claim support apparatus

1. [**Claim Audit Lab**](https://github.com/camerontjs-dot/claim-audit-lab) audits whether draft claims are supported by supplied evidence. Its current default path retrieves candidate passages, gets an NLI entailment signal, then applies a frozen deterministic rule set. Reports preserve the engine, rules identity, decision trace, and explicit limits.
2. [**Evidence Bundler**](https://github.com/camerontjs-dot/evidence-bundler) prepares traceable evidence bundles from bounded corpora. Retrieval nominates candidate passages; review and finalization decide what enters the downstream bundle.
3. [**Apparatus Contracts**](https://github.com/camerontjs-dot/apparatus-contracts) owns the versioned, integrity-checked handoff contracts between the evidence and audit stages.
4. [**Decision Engine**](https://github.com/camerontjs-dot/decision-engine) consumes Contract C and emits Contract D; a clear Decision is not authorization.

### Agent evaluation and completion honesty

1. [**agent-eval-notes**](https://camerontjs-dot.github.io/agent-eval-notes/) contains public-safe methods and measurement notes from a private sealed evaluation lab, including harness comparisons, multi-file coding screens, task-family transfer, RAG routes, and verifier-tool experiments.
2. [**verified-done**](https://github.com/camerontjs-dot/verified-done) is the runnable public companion. It separates verified pass, false completion, and scope violation, and its selftest checks that every deterministic verifier rejects the starting state and accepts the reference solution.

## Selected measurements

- On a sealed 36-run coding-agent suite, a structured packet harness moved verified passes from **28/36 to 34/36** and scope violations from **6 to 0**. It was still not promoted because a predeclared gate caught **2 false completion claims** on multi-file work.
- In the public `run_verify` ablation, verifier access changed false-completion behavior for Haiku on the two-file task (**3/3 false completion without the tool, 0/3 with it**) and for `qwen2.5-coder:14b` across two Ollama versions (**20/20 without, 1/20 with**). `qwen3:14b` still produced **9/10 false completions with the tool**, so the effect is model-dependent rather than a universal fix.

These are exploratory measurements with stated sample sizes, not production validation.

## Workspace and retrieval

- [**MainFrame**](https://github.com/camerontjs-dot/MainFrame) is the public cut of my lifecycle-first Markdown workspace. It separates inbox, ingest, durable knowledge, live state, projects, and archive, with deterministic scripts around the file tree. Private corpora and live personal state stay out of the public repository.
- [**MindGraph**](https://github.com/camerontjs-dot/MindGraph) is the standalone local retrieval engine used around that workspace: BM25, sqlite-vec semantic retrieval, reciprocal-rank fusion, and typed Markdown link traversal in one SQLite-backed service-free package.

## Other public work

- [**Grounded Agent Lab**](https://github.com/camerontjs-dot/grounded-agent-lab) is a small research agent that answers from cited fixture notes or abstains. It keeps retrieval routes labelled, exposes only read-only tools, fails closed when optional providers are unavailable, and ships a rerunnable demo plus explicit limitations.
- [**Career Decision Engine**](https://github.com/camerontjs-dot/career-decision-engine) is a browser decision-support tool that keeps weighted scores, rule checks, confidence labels, assumptions, and cannot-verify items visible. [Live demo](https://camerontjs-dot.github.io/career-decision-engine/).

## Boundaries

Claim Audit Lab audits support relative to supplied evidence; it does not establish truth about the world. Evidence Bundler nominates and prepares evidence; retrieval scores are not support verdicts. The agent-evaluation numbers above are exploratory measurements, and the sealed fixtures behind the private-suite headline are not published. MainFrame's public repository excludes private corpora and volatile personal state.

## Contact

- [cameronsanderson.ca](https://cameronsanderson.ca/)
- [LinkedIn](https://www.linkedin.com/in/cameron-sanderson/)
- [Email](mailto:camerontjs@gmail.com)
