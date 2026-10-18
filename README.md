# Software Architecture Patterns

A practical, diagram-rich field guide to software design and architecture patterns, distributed-systems principles, security, reliability, and runtime choices.

The guide explains what patterns do, the trade-offs they introduce, and when they are a good fit—or a poor one. It is intended as a learning and design-reference resource, not a set of rules to apply mechanically.

## Start here

- **[Browse the guide by strand and topic](index.md)** - home page and table of contents for the split guide.

## What’s covered

### Five architecture strands

1. **GoF Design Patterns** — creational, structural, and behavioral patterns.
2. **System Integration Patterns** — messaging, eventing, sagas, outboxes, and delivery reliability.
3. **Storage & Data Patterns** — analytical schemas, CQRS, event sourcing, caching, and data movement.
4. **Platform Infrastructure Patterns** — resilience, governance, deployment, and operations.
5. **Network Patterns** — network topologies, gateways, service discovery, service meshes, and mTLS.

### Cross-cutting topics

- **Pattern fit:** when to use and when to avoid each pattern.
- **Distributed-systems foundations:** CAP, PACELC, FLP, consistency models, delivery semantics, and other principles.
- **Runtime architectures:** bare metal, virtual machines, containers, serverless, PaaS, and WebAssembly.
- **Security Architecture:** identity, access control, data protection, threat modeling, secure delivery, detection, and recovery.
- **Quality attributes:** reliability, availability, integrity, and InfoSec architecture, including SLOs, RTO/RPO, and recovery design.

## How to use this guide

1. Start with the strand or quality attribute closest to the design problem.
2. Use the **when to use / when to avoid** tables to test whether a pattern addresses a real constraint.
3. Read the related foundations section for distributed behavior and consistency trade-offs.
4. Check the diagrams and review questions against the system’s actual failure modes, data, and operating model.
5. Record chosen guarantees, owners, recovery procedures, and assumptions in the system design.

Patterns are useful vocabulary and starting points. They do not replace requirements, threat modeling, operational experience, or validation against the target platform.

## Repository layout

```text
.
├── README.md
├── index.md                           # Split guide home page and TOC
├── strands/                           # Five architecture strands
└── topics/                            # Cross-cutting chapters
```

## Diagrams and Markdown

The guides use Mermaid diagrams. View them in a Markdown renderer that supports Mermaid, such as a compatible Git hosting interface or editor. A renderer without Mermaid support will still show the surrounding explanations and pattern tables.

## Scope and terminology

The catalog combines classic object-oriented patterns, enterprise integration patterns, cloud and platform practices, network designs, security controls, and distributed-systems results. These categories are related but not identical: some entries are formal theorems, some are design patterns, and some are operational practices.

Pattern names and guarantees can vary across platforms and literature. Where a design depends on a guarantee—such as ordering, consistency, failover, isolation, or exactly-once processing—define its scope explicitly and verify the implementation’s documented behavior.

## Contributing

Improvements are welcome when they make the guide more accurate, useful, and easy to navigate.

- Keep definitions concise and explain the problem each pattern addresses.
- Include benefits, costs, failure modes, and **when to use / when to avoid** guidance.
- Use Mermaid for diagrams that clarify relationships or flows; keep diagrams focused and valid.
- Prefer vendor-neutral explanations. Label platform-specific behavior when it matters.
- Distinguish formal results from rules of thumb and implementation patterns.
- Update the split chapter and single-file edition together when changing shared content.

## License

No license has been specified yet. Add a license before redistributing or accepting external contributions.
