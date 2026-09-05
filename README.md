# Cameron Sanderson

Eval and evidence systems for consequential workflows. Process before platform: reconstruct how one controlled workflow actually runs, then decide what to redesign, automate, or leave alone.

Primary offer on the site is **Controlled Automation Readiness** (about two weeks, one named workflow, a decision). Workflow Evidence Hardening is the method under that work, not a fifth product. Details: [cameronsanderson.ca](https://cameronsanderson.ca/).

Eight-plus years in sterile pharma lab and quality work (cGMP, USP <797>) is domain proof, not the product. Same habits in software: preserve source state, make failure modes testable, leave enough evidence for someone else to challenge the result.

Based in Ontario, Canada. Bilingual English and French.

## Method infrastructure on GitHub

These repos are inspectable worked objects for claim support and evidence handoff. They are not validated production systems.

1. [**Claim Audit Lab**](https://github.com/camerontjs-dot/claim-audit-lab) audits whether draft claims are supported by supplied evidence. Default path: retrieve candidates, NLI entailment signal, frozen deterministic rules. Reports keep engine, rules identity, decision trace, and explicit limits. Public record includes a v0.2 blind-gold failure; that stays visible on purpose.
2. [**Evidence Bundler**](https://github.com/camerontjs-dot/evidence-bundler) prepares traceable evidence bundles from bounded corpora. Retrieval nominates candidates; review decides what enters the bundle.
3. [**Apparatus Contracts**](https://github.com/camerontjs-dot/apparatus-contracts) owns the versioned, integrity-checked handoff contracts between evidence and audit stages.
4. [**Decision Engine**](https://github.com/camerontjs-dot/decision-engine) consumes Contract C and emits Contract D. A clear Decision is not authorization.

Related public notes: [agent-eval-notes](https://camerontjs-dot.github.io/agent-eval-notes/) and [verified-done](https://github.com/camerontjs-dot/verified-done) for completion honesty and harness measurement. [MainFrame](https://github.com/camerontjs-dot/MainFrame) and [MindGraph](https://github.com/camerontjs-dot/MindGraph) cover the local workspace and retrieval stack.

## Boundaries

Claim Audit Lab audits support relative to supplied evidence; it does not establish truth about the world. Evidence Bundler nominates and prepares evidence; retrieval scores are not support verdicts. None of these tools certify compliance or replace QA, validation, regulatory, or legal review.

## Contact

- [cameronsanderson.ca](https://cameronsanderson.ca/)
- [LinkedIn](https://www.linkedin.com/in/cameron-sanderson/)
- [Email](mailto:camerontjs@gmail.com)
