Jeff Smith

Backend & Platform Engineer

Identity-first infrastructure • Deterministic systems • Kubernetes-native design

Overview

I build backend and infrastructure systems where identity, authority, and runtime behavior are explicit, enforced, and verifiable.

My work focuses on:

Kubernetes-native workload identity (SPIRE / SPIFFE)
Admission and supply-chain enforcement
Deterministic validation pipelines
Durable authority attribution (PostgreSQL)
Observable backend systems (Prometheus, Tempo)

Systems are designed as bounded, self-contained slices with clear guarantees and failure modes.

I don’t assume systems are correct — I design them so they can prove they are.

System Design Lens

When designing distributed systems, I bias toward:

Workload identity over network trust
Explicit authority attribution for durable actions
Deterministic execution and validation layers
Fail-closed boundaries under uncertainty
Clear separation between infrastructure and application runtime

These principles ensure systems remain inspectable, enforceable, and predictable under real conditions.

Infrastructure Work

I build Kubernetes-based infrastructure systems focused on identity-first execution and policy enforcement.

Key areas:

Workload identity (SPIRE / SPIFFE)
Node and workload attestation (PSAT)
Digest-based admission enforcement
Internal registry containment
Identity-aware service communication (Istio mTLS + policy)

These systems are designed to make runtime behavior explicit and auditable, rather than implicit.

DevForge — Execution Integrity System

DevForge is a deterministic repository analysis system that answers:

Can this code be trusted to behave correctly under real conditions?

It evaluates execution reliability, not just static structure.

Key properties:

Deterministic classification (trustworthy, mixed-risk, untrustworthy)
Fail-closed behavior when signal quality is insufficient
Replay consistency enforcement (no stale or divergent results)
Detection of instability across repeated evaluations
Structured, explainable output tied to observable signals

DevForge is built to surface hidden failure modes such as:

non-deterministic execution
incomplete signal coverage
implicit dependencies
Backend Services

Application-layer systems focused on correctness and boundaries:

document-service
Deterministic validation and strict domain boundaries

job-processor-service
Async worker model with idempotency and explicit retry control

reservation-service
Transactional service with concurrency and integrity guarantees

Engineering Approach
Artifact-first engineering
Deterministic validation over assumptions
Fail-closed system design
Explicit boundaries over implicit behavior
Minimal surface area
Mechanical CI enforcement

AI tools accelerate implementation, but correctness and behavior are always deliberately designed and verified.

Current Focus
Backend and platform engineering roles
Identity-bound distributed systems
Deterministic validation and execution integrity
Infrastructure enforcement and containment
Contact

Email
sendtojeffsmith@gmail.com

GitHub
https://github.com/computeaholic
