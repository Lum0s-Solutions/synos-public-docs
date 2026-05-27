# Changelog

Public-facing release notes for Syn_OS. Format adapted from
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

This is the curated public changelog. It records milestones and the shape of the
work — not the internal subsystem mechanics, which live with the source ahead of
public release.

---

## [80.0.0] — 2026-05-22 — "Sunlance" (1.0 GA)

**The 1.0 general-availability release.** "Sunlance" closes the **v61 → v80
campaign** — twenty consecutive releases of compounding work — and marks the
point at which the platform's core is considered generally available.

### GA consolidation

- **ALFRED v6.0** — the AI daemon consolidated for GA. Local-first inference, no
  cloud in the critical path, with stronger guardrails around any autonomous
  behavior.
- **GRIMOIRE 1.0** — the training catalog reached 1.0: **108 hand-authored labs
  across 13 categories**, integrity-manifest enforced.
- **209-crate Rust workspace**, zero compile errors.
- **`synos-ops`** operator TUI expanded to a 23-tab dashboard.
- **Post-quantum by default** — hybrid ML-KEM / ML-DSA across the system's
  transport and signing surfaces, with SLH-DSA in the trust toolkit.

### Changed — kernel AI interface

- The earlier custom-syscall approach is **retired** — those numbers now collide
  with upstream Linux 6.19. The kernel AI/observability surface is now a
  **capability-gated, signed Rust kernel-module interface**: real, loadable,
  QEMU-boot-validated modules. Access is root-only and capability-gated, and the
  build hard-fails without a kernel signing key.

### The road to 1.0 (v61 → v80)

The GA is the sum of twenty releases. At a public level, the load-bearing themes:

- **Kernel AI interface re-architected and hardened** — signed modules, capability
  gates, root-only device access.
- **Post-quantum became the default**, not an option, across transport and signing.
- **Supply-chain trust deepened** — signed modules enforced, content-pinned
  packages, build-from-source attestation.
- **GRIMOIRE catalog matured to 1.0** — more labs, more categories, faction and
  cohort play hardened.
- **ALFRED consolidated to v6.0** — privacy-first posture, tighter guardrails.
- **Mesh opt-in** — consent-gated public-hive participation.

> The granular, per-subsystem record is intentionally not published here. Like the
> Operator image's capability surface (see [FEATURES.md](./FEATURES.md)), the
> mechanics of the platform's differentiating subsystems stay with the source
> ahead of public release.

---

## [60.x] — "Sun & Salt" (prior line)

The v60 "Sun & Salt" line was the prior public generation — a custom Linux 6.19
kernel with deep Rust integration, the ALFRED daemon, the GRIMOIRE training
platform, the Arcanum Hive mesh, post-quantum cryptography, and a self-healing,
reproducible build pipeline producing signed ISOs. v61 → v80 built on that
foundation to reach 1.0 GA.

---

*Own your infrastructure. Own your intelligence. Own your future.*
