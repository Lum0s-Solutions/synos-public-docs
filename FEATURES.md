# Capabilities

### *Syn_OS v80.0.0 "Sunlance" (1.0 GA) — what's actually inside.*

---

## kernel

- **Custom Linux 6.19** built with `CONFIG_RUST=y`.
- **Capability-gated kernel interface** — signed, memory-safe Rust kernel modules expose AI/observability state to userspace (decision telemetry, namespace trust, audit and incident signals, kernel-mitigation posture). Access is root-only and capability-gated; the build hard-fails without a kernel signing key.
- **Kernel hot path heavily Rust** (the post-Rust-ratchet commitment — hot paths and foundations move toward Rust, never away).
- **KSPP hardening fragment** merged into the kernel config.
- **Module signing enforced** — MOK keys, signed modules, signature verification at load.

---

## ALFRED — the AI daemon

- **ALFRED v6.0** — the GA consolidation of the daemon.
- **Local inference** via Ollama and ONNX. No cloud in the critical path.
- **11-region neuroanatomically-modeled brain.** Specialized regions coordinated by a brainstem.
- **Guardrails on autonomous behavior** — bounded, policy-checked remediation rather than free rein.
- **Cortex stage** fusing traditional AI, neuromorphic spike networks, quantum coherence collapse, and TNGS.
- **`research-mode` cargo feature** unlocks extended analysis paths for the Goodlife ISO.
- **Smoke-tested.** 14-check ALFRED smoke suite in CI.
- **Privacy-first.** No telemetry leaves the box without consent. The default state is silent.

---

## GRIMOIRE — gamified training

- **GRIMOIRE 1.0** catalog — **108 hand-authored labs** across **13 categories** (integrity-manifest enforced).
- **11 certification paths** mapped (Security+, OSCP, OSWE, CRTP, CRTO, eJPT, GPEN/GCIH, CEH, CISSP foundations, etc.).
- **Faction system** — at least three named houses, allegiance gates content, faction wars are a recurring beat.
- **XP economy** — earn, spend, craft, trade.
- **Boss contracts** — multi-stage scenarios chaining labs into multi-week arcs.
- **Branching narrative quests** with NPCs, cutscenes, and persistent world history.
- **5 competition modes** — leaderboard, squad missions, faction wars, head-to-head, asymmetric red-vs-blue.
- **Cohort mode** — class, club, and team-scale deployments.
- **First-boot wizard** — calibrated onboarding, not a personality test.
- **Sovereign Operator Path** — endgame arc graduating players to running their own mesh.

See [GRIMOIRE.md](./GRIMOIRE.md) for the deep dive.

---

## synos-bevy — game engine

- **Bevy 0.14** integration, ~7,000+ lines, **8 plugins**:
  - **Cutscene** — Season 1 narrative, async loading, typewriter UI, camera choreography.
  - **Mindmap** — force-directed 3D knowledge graph with RON persistence.
  - **Retro filter** — CRT post-processing with custom WGSL shaders.
  - **Cyberspace** — virtual world exploration, grid animation, particles.
  - **Skill tree** — Fallout-style perk chart with pentagon stat layout.
  - **Faction HQ** — three faction headquarters, NPC placement, mission boards, reputation system.
  - **Rehoboam** — Westworld-inspired 3D sphere system monitor.
  - **Twin** (v51 Storm Glass) — kernel-state visualization plugin.

---

## Arcanum Hive — distributed mesh

- **8-node target topology** with Tailscale (WireGuard fallback).
- **Kubernetes operator** managing `ArcanumNode` lifecycle, `SecurityAlert` CRDs, phase state machines.
- **mTLS by default.** Per-tenant HMAC.
- **Stoneglass Ansible playbook** (v55) — public self-hosting recipe.
- **Remote node attestation** — kernel version, SSH hardening, SUID audit, CVE scan.

---

## post-quantum cryptography (default)

Post-quantum is the **default posture**, not an opt-in — hybrid key exchange and signatures across the system's transport and signing surfaces.

- **ML-KEM** — key encapsulation (Kyber successor).
- **ML-DSA** — digital signatures (Dilithium successor).
- **SLH-DSA** — hash-based signatures (SPHINCS+ successor).
- Integrated through the project's `Icarus` crate.

---

## supply chain

- **SBOM (CycloneDX)** generated per ISO profile.
- **Cosign-signed releases** with Rekor transparency log entries.
- **SLSA-3 reproducible build pipeline** with dual-witness cross-oracle verification (when the second oracle is online).
- **`cargo deny` clean** — OpenSSL/native-tls banned. Unmaintained crates pinned or replaced.
- **Patch generator** — block-level binary diffing with zstd compression and SHA-256 manifests.
- **Lab integrity manifest** — every lab in the 108-lab corpus hashed and verified.

---

## desktop experience

- **Cinnamon + Xfce4 dual-desktop** support out of the box.
- **LightDM** display manager.
- **Plymouth** boot splash with the project's red-phoenix theme.
- **synos-ops TUI** — expanded multi-tab operations dashboard for the operator.
- **Sound theme**, custom wallpapers, fastfetch integration.
- **Branding consistency** across MOTD, terminal headers, and `/etc/os-release`.

---

## tooling

- **600+ native security tools** via pacman/AUR.
- **3,400+ tools available** through Distrobox containers (Kali, BlackArch, Parrot images).
- **Fully curated** — the point is what you can do, not how many binaries are in `/usr/bin`.
- **Offensive tooling boundaries are mechanical** — what's available in each ISO is what's intended.

---

## quality gates

- **209-crate Rust workspace.** Zero compile errors.
- **1,600+ tests.** 100% pass rate.
- **35% tarpaulin coverage floor**, ratcheted upward over time.
- **SHA-pinned CI workflows** across hosted and self-hosted runners.
- **Self-healing build pipeline** across 41 stages.
- **MkDocs Material** documentation site, version-aware.

---

## what isn't on this list

The Operator (Master) image's full capability surface — the proprietary Fragment Field IDS, the full C2 framework, the unrestricted offensive tooling layer, the federation server internals, the license-gate enforcement mechanism. Those exist. They aren't part of the public release.

What's listed above is what GRIMOIRE Public + Goodlife users will actually have in hand when those ISOs drop.
