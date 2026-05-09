# Capabilities

### *Syn_OS v60.0.0 "Sun & Salt" — what's actually inside.*

---

## kernel

- **Custom Linux 6.19** built with `CONFIG_RUST=y`.
- **17 custom system calls** (469–485) exposing AI/consciousness state, eBPF instrumentation, kernel observability, and process attestation to userspace.
- **11 loadable Rust kernel modules**: memory, networking, hardening, interrupts, modloader, procfs, power, consciousness, hardening, module verification, plus the synos hardening core.
- **Kernel hot path 83.54% Rust** (post-v56 Rust ratchet).
- **KSPP hardening fragment** merged into the kernel config.
- **Module signing** wired through MOK keys generated at build time.

---

## ALFRED — the AI daemon

- **Local inference** via Ollama and ONNX. No cloud in the critical path.
- **11-region neuroanatomically-modeled brain.** Specialized regions coordinated by a brainstem.
- **Cortex stage** fusing traditional AI, neuromorphic spike networks, quantum coherence collapse, and TNGS.
- **`research-mode` cargo feature** unlocks extended analysis paths for the Goodlife ISO.
- **Smoke-tested.** 14-check ALFRED smoke suite in CI.
- **Privacy-first.** No telemetry leaves the box without consent. The default state is silent.

---

## GRIMOIRE — gamified training

- **100 hand-authored labs** across **13 categories** (integrity-manifest enforced).
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

## post-quantum cryptography

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
- **Lab integrity manifest** — every lab in the 100-lab corpus hashed and verified.

---

## desktop experience

- **Cinnamon + Xfce4 dual-desktop** support out of the box.
- **LightDM** display manager.
- **Plymouth** boot splash with the project's red-phoenix theme.
- **synos-ops TUI** — 6-tab operations dashboard for the operator.
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

- **160-crate Rust workspace.** Zero compile errors.
- **1,600+ tests.** 100% pass rate.
- **35% tarpaulin coverage floor**, ratcheted upward over time.
- **17 CI workflows** — 5 ubuntu-latest, 12 self-hosted runners.
- **Self-healing build pipeline** across 41 stages.
- **MkDocs Material** documentation site, version-aware.

---

## what isn't on this list

The Operator (Master) image's full capability surface — the proprietary Fragment Field IDS, the full C2 framework, the unrestricted offensive tooling layer, the federation server internals, the license-gate enforcement mechanism. Those exist. They aren't part of the public release.

What's listed above is what GRIMOIRE Public + Goodlife users will actually have in hand when those ISOs drop.
