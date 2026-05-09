# Architecture

### *biological in inspiration. rigorous in implementation. v60.0.0 "Sun & Salt".*

---

## the synaptic gap

The design philosophy starts with a metaphor and refuses to let it become decorative. A synapse is the cleft between two neurons — the gap where electrical signal becomes meaning, where pre-synaptic firing crosses through chemistry into post-synaptic decision.

Syn_OS treats the operating system itself as the synaptic cleft.

```
Pre-synaptic neuron    = Hardware
Synaptic cleft         = Syn_OS (kernel + userspace + ALFRED)
Post-synaptic neuron   = Application consciousness (ALFRED decisions, user processes)
Neurotransmitters      = System calls (469–485)
Receptors              = Syscall handlers
Synaptic plasticity    = Adaptive kernel module behavior + ALFRED's learning loops
```

This is not branding. It's the framing every architectural decision is checked against.

---

## the four pillars

### the kernel

A custom Linux 6.19 build with `CONFIG_RUST=y` and **17 custom system calls** (469–485). The syscalls expose:

| Range | Purpose |
|---|---|
| **469–479** | Consciousness state, quantum memory entanglement, AI metrics, eBPF monitor control |
| **480–485** | Kernel observability, perf instrumentation, process attestation, snapshot, twin |

The kernel ships **11 loadable Rust kernel modules** covering memory, networking, hardening, interrupts, modloader, procfs, power, consciousness, and module verification. After the v56 Rust Ratchet, the kernel hot path is **83.54% Rust** by line count. KSPP hardening fragment merged. Module signing wired through MOK keys generated at build time.

### ALFRED

The Adaptive Learning Framework for Responsive Evolution and Defense. ALFRED is the AI daemon — not a chatbot, but the operator's companion at the system level.

- **11-region neuroanatomical brain.** Modeled loosely after biological structure: thalamus (gating), amygdala (threat detection), hippocampus (memory), insula (interoception), cerebellum (coordination), corpus callosum (interhemispheric routing), default mode network (idle synthesis), glial (support), brainstem (orchestration), nucleus, plus the consciousness-types crate that ties them.
- **Cortex stage** fuses traditional AI, neuromorphic spike networks, quantum coherence collapse, and Edelman's Theory of Neuronal Group Selection (TNGS) into a single decision pipeline.
- **Local inference** via Ollama and ONNX. No cloud in the critical path.
- **BrainBridge** consumes `AlfredSignal` events from kernel telemetry into the cortex. The kernel and the daemon talk through the syscall surface.

### GRIMOIRE

The gamified cybersecurity training platform — 100 labs, 13 categories, faction system, XP economy, boss contracts, branching narrative, cohort competition. Covered in detail in [GRIMOIRE.md](./GRIMOIRE.md).

GRIMOIRE is the public face. It's what the GRIMOIRE Public ISO ships. It's the apprenticeship surface for the entire community we're building.

### the mesh — Arcanum Hive

When the system extends across hardware, it does so as the Arcanum Hive: an 8-node Tailscale mesh coordinated by a Kubernetes operator. Per-tenant HMAC. mTLS by default. Sovereignty as a design property, not a marketing claim.

The Hive Stoneglass GA playbook (v55) is the public-facing self-hosting recipe. The hive is yours to extend.

---

## the three-image strategy

Syn_OS is built once and ships in three signed ISOs from a single source tree.

| Image | Audience | License |
|---|---|---|
| **Operator (Master)** | The team. Internal. | Proprietary, not distributed publicly |
| **GRIMOIRE Public** | Students, cohorts, practitioners | Apache 2.0 + LicenseRef-GRIMOIRE-Public |
| **Goodlife** | AI researchers, post-quantum, civilian work | Apache 2.0 |

Capability boundaries between images are **mechanically enforced** — by binary symbol scanning, feature flag audits, lab integrity manifests, and supply-chain provenance checks. The mechanism is part of the architecture, not bolted on.

---

## the substrate

Below the four pillars sits the engineering work that makes the higher-level vision viable:

- **160-crate Rust workspace** with zero compile errors. `cargo check --workspace` passes; `cargo deny` clean.
- **Toolchain pinned** at `nightly-2026-02-12` (rustc 1.95.0-nightly).
- **41-stage self-healing build pipeline.** Producing the three images is a multi-hour process that recovers from individual stage failures without losing the whole run. SLSA-3 reproducible build target. Dual-witness signature support across mesh nodes.
- **Test infrastructure.** 1,600+ tests. 100% pass rate. 35% tarpaulin coverage floor. Continuous integration across 17 workflows (5 ubuntu-latest, 12 self-hosted).
- **Post-quantum cryptography.** ML-KEM (key encapsulation), ML-DSA (signatures), SLH-DSA (hash-based signatures) integrated into the trust toolkit.
- **Cosign + Rekor** signing path for ISO releases. Sigstore transparency log entries. Verifiable provenance from build oracle to USB stick.
- **MkDocs Material documentation** site, version-aware, fact-checked against the source tree.

---

## design axioms

Three axioms applied recursively:

1. **The synaptic gap is real.** Hardware is not the OS. The OS is not the application. The OS is the gap, and the quality of the system is the quality of that translation.
2. **Memory safety where it matters.** The Rust ratchet is a one-way commitment. Kernel hot paths and userspace foundations move toward Rust, never away.
3. **Tiers are mechanical.** Capability boundaries between Operator, GRIMOIRE Public, and Goodlife images are enforced by the build, not by goodwill.

---

## further reading

The deeper architectural surface — full kernel internals, ALFRED's brain crate topology, mesh authentication and rotation mechanics, the master-only capability set — lives with the source. The public-facing pillars described here are the shape of the system.

The shape is enough to know whether the rest will interest you.
