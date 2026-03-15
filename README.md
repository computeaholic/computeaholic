Jeff Smith

Backend & Platform Engineer

Identity-first infrastructure • Durable backend systems • Kubernetes-native design

Overview

I build backend and infrastructure systems where identity, authority, and runtime behavior are explicit and inspectable.

My work focuses on:

Kubernetes-native identity (SPIRE / SPIFFE)

Admission and supply-chain enforcement

Durable authority attribution (PostgreSQL)

Observable backend systems (Prometheus)

Explicit architectural boundaries

Systems are decomposed into bounded, self-contained slices that demonstrate both capabilities and limits.

System Design Lens

When designing distributed systems I prioritize:

Workload identity over network trust

Explicit authority attribution for durable actions

Deterministic infrastructure layers

Fail-closed security boundaries

Clear separation between infrastructure and application runtime

These principles shape the ThreadForge architecture, which decomposes platform infrastructure into explicit layers.

ThreadForge Architecture

ThreadForge is a layered platform architecture for executing distributed services and AI agents using workload identity, service mesh authentication, and policy-driven communication boundaries.

Agents / Workloads
        ↓
Containment Surface
        ↓
Secure Runtime
        ↓
Identity Surface
        ↓
Fabric

Reference architecture:

https://github.com/computeaholic/threadforge-reference-architecture

Infrastructure Repositories
threadforge-fabric

Minimal Kubernetes substrate providing:

internal container registry

SPIRE identity plane

PostgreSQL stateful store

Prometheus monitoring

https://github.com/computeaholic/threadforge-fabric

threadforge-identity-surface

Workload identity and admission enforcement surface:

SPIRE server and agents

PSAT-based node attestation

digest-based admission enforcement

https://github.com/computeaholic/threadforge-identity-surface

threadforge-secure-runtime

Identity-gated backend runtime:

SPIRE-issued workload identity

durable authority ledger (PostgreSQL)

Prometheus metrics exposure

https://github.com/computeaholic/threadforge-secure-runtime

threadforge-containment-surface

Containment validation harness demonstrating:

admission enforcement

supply-chain policy enforcement

bounded authority claims

https://github.com/computeaholic/threadforge-containment-surface

Backend Services

These repositories demonstrate application-layer backend design patterns.

document-service

Deterministic validation and domain boundary design.

job-processor-service

Async worker system demonstrating retry boundaries and idempotency.

reservation-service

Transactional service demonstrating concurrency control and correctness guarantees.

Engineering Approach

Artifact-first engineering

Fail-closed infrastructure

Explicit architectural boundaries

Minimal surface area

Mechanical CI enforcement

AI tools are used to accelerate disciplined implementation — not replace engineering judgment.

Current Focus

Backend and platform engineering roles

Identity-bound distributed systems

Infrastructure architecture and containment models

Contact

Email
sendtojeffsmith@gmail.com

GitHub
https://github.com/computeaholic
