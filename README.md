## Cameron Sanderson

Self-taught applied AI systems builder from regulated sterile pharma QA/QC. Eight plus years in manufacturing under cGMP, GLP/GDP, USP <797>, Health Canada, and FDA 21 CFR 210/211. The same operating style I use for deviations, CAPA, and validation now drives how I build AI tools: traceability, failure-mode thinking, explicit uncertainty, and quality gates before outputs are trusted.

Based in Richmond Hill, Ontario. Bilingual English and French.

### What I build

I design and build local AI workflow systems where provenance, structured outputs, validation sweeps, and confidence calibration keep the result from overclaiming what the inputs support. I work by directing and reviewing model-generated code and am actively building direct Python proficiency.

Most of what follows is public. The repos are the evidence.

### Research apparatus

The strongest public project cluster is a multi-component evidence-support apparatus for a narrow question: how do we keep AI-assisted research workflows from carrying unsupported claims into final outputs?

Three public repos form the current apparatus:

[**Evidence Bundler**](https://github.com/camerontjs-dot/evidence-bundler) consumes scaffold-run artifacts, nominates candidate evidence passages through BM25, hybrid, reranked, and contradiction retrieval, then carries those nominations through review annotation, excerpt refinement, finalization, and coverage reporting. 192 tests. Real-corpus demo against FDA CGMP guidance.

[**Claim Audit Lab**](https://github.com/camerontjs-dot/claim-audit-lab) consumes evidence bundles and produces deterministic claim-support audit verdicts. Rule-based, not model-scored. 136 tests.

[**Apparatus Contracts**](https://github.com/camerontjs-dot/apparatus-contracts) is the versioned handoff specification that connects the three components. Controlled vocabulary, schema definitions, hash-verified integrity checks, and a Python verifier suite. Regulated-industry data-integrity grammar (ALCOA+, 21 CFR Part 11) applied to AI workflow tooling.

The components communicate through locked contract artifacts, not shared code. Each repo tests independently and verifies intake from the upstream component at its own boundary.

### Knowledge layer

The second pairing is a personal knowledge system built in two parts that complement each other.

[**Mainframe**](https://github.com/camerontjs-dot/MainFrame) is a Markdown-first knowledge workspace organized by information lifecycle: inbox, ingest, knowledge, live state, projects, archive. Each stage has its own update rules and deterministic routing scripts. The structure is the retrieval surface.

[**MindGraph**](https://github.com/camerontjs-dot/MindGraph) is the local retrieval engine that indexes Mainframe. One SQLite file, no service. BM25 plus sqlite-vec cosine fused with Reciprocal Rank Fusion, a typed `[[link]]` document graph with bounded expansion walks, and an MCP server for local clients. 97 tests.

Mainframe organizes the notes. MindGraph makes them findable.

### Other public tools

[**Basic Research Harness**](https://github.com/camerontjs-dot/basic-research-harness) is a small agent-engineering learning piece that builds the same research-to-bundle workflow two ways: a raw Python agent loop that owns every decision point in code, and a Claude Code SDK rebuild that moves the procedure, review step, and QA gate into project assets (Skill, sub-agent, PostToolUse hook). Putting the two side by side makes the responsibilities of an agent harness visible.

[**Career Decision Engine**](https://github.com/camerontjs-dot/career-decision-engine) is a browser-based decision-support tool for comparing job offers and career paths. Relative scoring, rule checks separated from the weighted score, calibrated confidence labels, and a guided intake. 6,309 checks across 700 evaluated comparisons. [Live demo.](https://camerontjs-dot.github.io/career-decision-engine/)

[**Tripwire**](https://github.com/camerontjs-dot/Tripwire) is a local-first template that turns an AI coding agent into a personal research analyst and portfolio skeptic. Provenance, disconfirming evidence, calibrated language, validation hooks, and an append-only audit log. Agent-neutral, tested with Claude, Codex, and Gemini.

### Private systems

Two larger systems are in active use but not yet public. I can walk through the architecture without exposing sensitive content.

- **Command Center** is a local multi-context AI workflow system with 7+ specialized analyst modes, structured outputs, provenance, and scope control.
- **The Registered Edge** is a content workflow with 20+ custom skill modules for research synthesis, drafting, review, formatting, and quality control. Designed to reduce AI-tell writing, surface uncertainty, and separate human judgment from model-generated support.

### Where I am calibrated

I have not published formal ML research. My evidence is execution-based rather than credential-based, and my strongest contribution to AI work is the validation posture I bring from regulated quality environments. Python is a growing strength, not a finished senior-engineering claim. The public portfolio speaks for itself, and I am still expanding it.

### Contact

- LinkedIn: [linkedin.com/in/cameron-sanderson](https://www.linkedin.com/in/cameron-sanderson/)
- Email: camerontjs@gmail.com
