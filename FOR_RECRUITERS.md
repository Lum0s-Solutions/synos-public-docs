# Professional Showcase

### *Ty Limoges, lead of Syn_OS — a snapshot of the work that produced v80.0.0 "Sunlance", the 1.0 GA release.*

---

## the project

**Syn_OS** is a multi-year, full-stack cybersecurity operating system project conceived, architected, and led by Ty Limoges out of LumOs Solutions. It is not a fork. It is not a theme on top of an existing distribution. It is a from-scratch operating system platform that takes itself seriously across:

- Custom Linux kernel engineering
- A 209-crate Rust workspace
- Local AI daemon design and integration
- A gamified training environment with 108 hand-authored labs
- A distributed, encrypted-by-default mesh
- A 41-stage self-healing build pipeline
- Post-quantum cryptography integration
- Game engine integration via Bevy 0.14
- Documentation craft at production quality

It is the kind of project that exercises the full stack and refuses to ship at a quality bar lower than the one its own gates enforce.

---

## the v80 numbers

| Metric | Value |
|---|---|
| Version | **v80.0.0** "Sunlance" — **1.0 GA** |
| Release campaign | **20 consecutive versions** (v61 → v80) to GA |
| Cargo workspace | **209 active crates**, 0 compile errors |
| Kernel AI/observability interface | Signed, capability-gated Rust kernel modules (root-only) |
| Kernel hot-path Rust | Majority Rust (one-way Rust-ratchet commitment) |
| AI daemon | **ALFRED v6.0**, local-only inference |
| GRIMOIRE labs | **108** hand-authored, manifest-enforced (**catalog 1.0**) |
| Lab categories | **13** |
| Bevy game engine plugins | **8** |
| ISO profiles | **3** (Operator / GRIMOIRE Public / Goodlife) |
| Build pipeline | self-healing, multi-stage |
| Post-quantum crypto | **default** (hybrid ML-KEM / ML-DSA, SLH-DSA) |
| Supply chain | SBOM per ISO, Cosign + Rekor, SLSA build-from-source attestation |
| Documentation | version-aware, fact-checked against source |

---

## the disciplines exercised

- **Kernel-level systems engineering.** Custom Linux 6.19 build with `CONFIG_RUST=y`. A capability-gated, signed-module interface exposing AI/observability state to userspace (the GA re-architecture of the kernel AI surface). KSPP hardening. MOK module signing enforced. Kernel observability instrumentation (eBPF, perf, attestation hooks).
- **Rust at scale.** 209-crate workspace with deliberate architectural separation. `cargo deny` clean (OpenSSL/native-tls banned). Sustained discipline around dependency hygiene and supply-chain posture.
- **AI/ML integration.** Local-first inference via Ollama and ONNX. An 11-region neuroanatomically-modeled brain daemon (ALFRED). Cortex stage fusing traditional AI, neuromorphic spike networks, quantum coherence, and TNGS into a unified decision pipeline. No cloud in the critical path.
- **Game design and engine integration.** Bevy 0.14 integration across 8 plugins (~7,000+ lines). Cutscenes, mindmaps, retro filters, cyberspace exploration, skill trees, faction HQs, system monitors, kernel-state visualization.
- **Distributed systems.** 8-node Tailscale mesh (WireGuard fallback) coordinated through a Kubernetes operator. mTLS + per-tenant HMAC. Cross-oracle build verification for SLSA-3 dual-witness signatures.
- **Post-quantum cryptography.** ML-KEM, ML-DSA, SLH-DSA integrated into the trust toolkit through the project's `Icarus` crate.
- **Build engineering.** 41-stage, self-healing, multi-hour pipeline producing three signed ISOs from a single source tree, with mechanical enforcement of capability boundaries between images.
- **Compliance and supply chain.** SBOM (CycloneDX) per ISO. Cosign + Rekor signing. SLSA-3 reproducible build target. FedRAMP Moderate control map (v59 Doublecross). Daily continuous monitoring.
- **Documentation craft.** MkDocs Material site, version-aware, checked against the source tree. Operator runbooks. Stage-by-stage build-wizard pedagogy.

---

## the way of working

- **Quality bar held high.** Test coverage taken seriously. Continuous integration treated as load-bearing rather than ceremonial. Reproducibility, supply-chain provenance, and binary boundary enforcement engineered in rather than hoped for.
- **Long-arc discipline.** Multi-year sustained execution. Eighty version releases to a 1.0 GA. The v61 → v80 campaign coordinated twenty consecutive releases into a single coherent general-availability surface.
- **Solo-led, multi-perspective.** Architectural through-line carried by the lead, with disciplined coordination across the disciplines listed above.
- **Documentation as code.** Living documents. Version-aware. The kind of documentation that holds up under actual use because it's checked against the source.

---

## what this evidences

For anyone evaluating cybersecurity, AI, or systems engineering candidates: the body of work here demonstrates the ability to hold a complex, multi-disciplinary project across a long arc, to make architectural decisions that compound rather than collapse, and to sustain quality without the scaffolding of a large team.

For anyone evaluating leadership: a project of this scope cannot be willed into existence. It requires opinionated technical taste, disciplined prioritization, mechanical enforcement of standards, and a sustained appetite for the unglamorous work — building, repairing, documenting, and refining the same systems over years until they hold up.

---

## further reading

- [README.md](./README.md) — what Syn_OS is and what's in v80
- [GRIMOIRE.md](./GRIMOIRE.md) — the gamified training platform
- [ARCHITECTURE.md](./ARCHITECTURE.md) — the four pillars and the substrate
- [FEATURES.md](./FEATURES.md) — capability inventory
- [ROADMAP.md](./ROADMAP.md) — what's shipped and what's coming
- [CHANGELOG.md](./CHANGELOG.md) — public release notes, v80 GA

---

If any of the above aligns with what you're looking for — in a hire, in a partner, in a research collaborator — we'd be glad to have the conversation.

**Last updated:** 2026-05-27
