Jeff Smith
Backend & Platform Engineer

Identity-first infrastructure • Durable backend systems • Kubernetes-native design

Overview

I build backend and infrastructure systems where identity, authority, and runtime behavior are explicit and inspectable.

Most of my work sits at the intersection of:

Kubernetes-native identity (SPIRE / SPIFFE)
Admission and supply-chain enforcement
Durable authority attribution (PostgreSQL)
Observable backend systems (Prometheus)
Explicit architectural boundaries

I prefer to break systems into small, bounded slices that make both capabilities and limits obvious. Each system is designed to be independently verifiable.

System Design Lens

When I design distributed systems, I bias toward:

Workload identity over network trust
Explicit authority attribution for durable actions
Deterministic infrastructure layers
Fail-closed security boundaries
Clear separation between infrastructure and application runtime

These principles guide how I structure both infrastructure and backend services.

Infrastructure Work

I’ve been building a set of Kubernetes-based infrastructure slices focused on identity-first execution and policy enforcement.

These systems explore:

Workload identity using SPIRE / SPIFFE
Node and workload attestation (PSAT)
Digest-based admission enforcement
Internal registry containment
Identity-aware service communication (Istio mTLS + policy)

The goal is to make runtime behavior explicit, enforceable, and auditable rather than assumed.

Backend Services

These repos focus on application-layer patterns:

document-service
Deterministic validation and domain boundaries

job-processor-service
Async worker model with retry + idempotency guarantees

reservation-service
Transactional service with concurrency control

Engineering Approach
Artifact-first engineering
Fail-closed infrastructure
Explicit boundaries over implicit behavior
Minimal surface area
Mechanical CI enforcement

I use AI tools to move faster, but all systems are designed and validated deliberately.

Current Focus
Backend / platform engineering roles
Identity-bound distributed systems
Infrastructure and containment design
Contact

Email
sendtojeffsmith@gmail.com

GitHub
https://github.com/computeaholic
