# Jeff Smith

**Systems builder focused on identity, assurance, and making software prove what it claims.**

I build infrastructure and software systems where authority is explicit, failure is observable, and important claims are backed by executable evidence rather than configuration or documentation alone.

A lot of my work lives around Kubernetes, workload identity, software supply-chain controls, deterministic validation, and the uncomfortable question:

> How do you know the system actually did what you think it did?

That question has pulled me pretty far down the rabbit hole.

---

## TruthFast

My current flagship project is **[TruthFast](https://github.com/computeaholic/TruthFast)**, an executable assurance reference architecture for identity-bound consequential execution.

TruthFast combines:

- SPIFFE / SPIRE workload identity
- Kubernetes and policy enforcement
- software supply-chain integrity
- fail-closed behavior
- deliberate positive and negative execution
- producer-owned evidence
- non-healing active assurance
- deterministic proof
- correlated observability
- exact-source runtime qualification

The central idea is simple:

> **The unit of assurance is not the component. It is the justified conclusion about an identity-bound operation.**

The system is intentionally built so that proof cannot quietly repair the state it is evaluating. Failure, blocked execution, denial, trust continuity, evidence integrity, and recovery are meant to be exercised rather than assumed.

TruthFast V1 was reconstructed from source through a destructive Golden Boot, exercised through its supported demonstrations and failure witnesses, and qualified against an exact source revision.

The architecture paper is publicly citable:

**TruthFast: Constitutional Assurance for Identity-Bound Consequential Execution**  
DOI: **10.5281/zenodo.22548396**

TruthFast is source-available under the PolyForm Perimeter License 1.0.1. Certain mechanisms are patent pending.

---

## DevForge

**DevForge** grew out of a related question:

> Can a repository demonstrate that its behavior is trustworthy under real conditions?

It is a deterministic repository-analysis and execution-integrity system designed to surface things that ordinary static inspection can miss:

- nondeterministic behavior
- incomplete evidence
- stale or divergent evaluation
- hidden dependencies
- unstable execution
- unjustified confidence

The emphasis is not on generating another score. It is on making the reasoning behind a conclusion inspectable.

---

## How I think about systems

I tend to reach for the same principles regardless of the implementation:

**Identity before location.**  
Network position is not authority.

**One owner for a state transition.**  
Observers and consumers should not quietly become alternate authorities.

**Failure should stay failure.**  
Unavailable, blocked, denied, and failed are different facts and should remain different facts.

**Evidence should come from the thing that owns the truth.**  
A dashboard or verifier should not manufacture the state it later claims to have observed.

**Determinism where meaning matters.**  
Distributed systems contain legitimate variability. Security-bearing differences should not disappear inside that variability.

**Break things deliberately.**  
A fail-closed claim is much more interesting after the dependency has actually failed.

---

## Building with AI

A significant part of my recent work has been exploring what becomes possible when AI is treated as a serious engineering collaborator rather than a code-completion tool.

My workflow is highly iterative:

1. reason about the problem and architecture,
2. turn the architecture into executable contracts,
3. build quickly,
4. attack the implementation,
5. preserve the evidence,
6. repair the first incorrect assumption,
7. repeat until the system earns the claim.

AI accelerates implementation, research, hostile review, and iteration. It does not replace the responsibility to decide what the system should mean or to verify that reality matches the design.

TruthFast and DevForge are products of that process.

---

## Technical territory

Most of my recent work touches some combination of:

- Kubernetes
- SPIFFE / SPIRE
- workload identity and attestation
- Istio
- admission and authorization policy
- software supply-chain security
- container registries and artifact integrity
- Python
- Go
- PostgreSQL
- Prometheus / Loki / Tempo / Grafana
- deterministic validation
- distributed-system failure semantics
- security research and adversarial testing

I also maintain smaller backend systems exploring transactional correctness, idempotent workers, validation boundaries, and concurrency.

---

## What I am interested in

I am especially interested in work involving:

- software and infrastructure assurance
- identity-first distributed systems
- security architecture
- high-consequence systems
- platform engineering
- research engineering
- technical consulting
- AI-augmented engineering workflows
- problems where “it probably works” is not an acceptable answer

I like difficult systems, skeptical reviewers, and problems where the details matter.

---

## Contact

**Email:** [sendtojeffsmith@gmail.com](mailto:sendtojeffsmith@gmail.com)

**GitHub:** [github.com/computeaholic](https://github.com/computeaholic)

**TruthFast:** [github.com/computeaholic/TruthFast](https://github.com/computeaholic/TruthFast)

**TruthFast paper:** [doi.org/10.5281/zenodo.22548396](https://doi.org/10.5281/zenodo.22548396)
