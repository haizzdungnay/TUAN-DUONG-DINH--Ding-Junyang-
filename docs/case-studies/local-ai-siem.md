# Local AI SIEM Analyzer — Security Engineering & AI Integration

[← Back to portfolio](../../README.md) · [Source repository](https://github.com/haizzdungnay/local-ai-siem-analyzer)

**Focus:** Detection-support tooling, local LLM orchestration, secure data handling  
**Stack:** Python, Wazuh, Ollama, ChromaDB, VMware, Docker

## Problem and scope

Security alerts can be difficult to interpret consistently without context about the triggering rule, supporting events and probable next steps. This project builds a **local AI-assisted analyst tool** around Wazuh alerts; it does **not** claim to replace a SIEM, replace analyst judgment, or autonomously remediate incidents.

The repository credits the original team members. My stated contribution covers application implementation and integration; the original academic/team attribution remains in the project README.

## Engineering approach

- Read time-bounded alert information from the Wazuh Indexer and prepare structured context for analysis.
- Use an Ollama-hosted local model to produce analyst-facing summaries and suggested next checks.
- Retrieve relevant rule/MITRE context rather than treating a language model response as a source of truth.
- Separate facts, inferences, uncertainty and limitations in the analyst interface.
- Keep credentials server-side and avoid passing unfiltered raw log payloads into the LLM.
- Provide repeatable test and lab workflows for development without requiring live security infrastructure for every test.

## Public evidence

| What to examine | Direct evidence |
| --- | --- |
| Architecture and setup | [Project README](https://github.com/haizzdungnay/local-ai-siem-analyzer/blob/main/README.md) · [Network design](https://github.com/haizzdungnay/local-ai-siem-analyzer/blob/main/docs/network.md) |
| Analysis implementation | [AI module](https://github.com/haizzdungnay/local-ai-siem-analyzer/tree/main/ai_module) |
| Security governance | [Security governance](https://github.com/haizzdungnay/local-ai-siem-analyzer/blob/main/docs/security-governance.md) |
| CI verification | [Python tests workflow](https://github.com/haizzdungnay/local-ai-siem-analyzer/blob/main/.github/workflows/python-tests.yml) · [Recent Actions](https://github.com/haizzdungnay/local-ai-siem-analyzer/actions) |
| Evaluation approach | [Evaluation materials](https://github.com/haizzdungnay/local-ai-siem-analyzer/tree/main/eval) |

## Validation and limitations

The repository has a Python CI workflow with tests, tracked-secret checks, dependency-audit checks and SBOM generation; the workflow history includes successful runs. This does **not** establish a universal detection rate, hallucination-free outputs or enterprise production readiness.

LLM output is advisory, not a confirmed incident verdict. The documented evaluation set and test artifacts should be consulted for scope-specific performance claims; none are invented here.

## Interview discussion topics

Alert provenance; trustworthy retrieval; sensitive-log minimization; offline model trade-offs; analyst verification; hallucination/uncertainty handling; and reproducible test evidence.

---

*The repository is a team-labelled project; the case study documents the engineering work and verifiable public artifacts without erasing original team credits.*