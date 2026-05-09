# Roadmap

### *what's shipped, what's imminent, what's the long game.*

---

## v60.0.0 "Sun & Salt" — current

The first ISO carrying the full v44 → v60 codesprint. Sixteen versions of compounding work fused into one signed release.

**What v60 brings:**
- SBOM (CycloneDX) drift detector across builds
- IPO readiness self-test — institutional-grade audit pass
- External blocker playbook for cosign + cross-oracle ceremonies
- All v44–v59 features merged into a single coherent release surface

---

## the v44 → v60 codesprint, shipped

| Codename | What landed |
|---|---|
| **v44 Crucible** | Fuzz harness, attest LSM, observability kernel, rebuild-verify CI |
| **v45 Glasswalker** | Kernel observability syscalls 480–485 (now 17 total) |
| **v46 Beachhead** | Process attestation HMAC ledger + LSM hooks |
| **v47** | License gate, audit HMAC chain, CSV/EVTX/syslog exports |
| **v48 Forge** | Sigstore Rekor + SLSA-3 reproducible builds |
| **v49 Crystal Net** | Federation server (mTLS + per-tenant HMAC) |
| **v50 Tenfold** | RaaS engine, billing integration, LLM red-team harness |
| **v51 Storm Glass** | TwinPlugin (8th synos-bevy plugin) + kernel-snapshot |
| **v52 Riftrunner** | In-kernel safe-bytecode VM |
| **v53 Quantumweave** | synos-cortex-q tensor-network ML |
| **v54** | Capability tokens (synos-curtain-tokens) |
| **v55 Stoneglass** | Hive Ansible deploy (8-node GA playbook) |
| **v56** | Rust ratchet — kernel hot-path Rust at 83.54% |
| **v57 Phoenix Eye** | LLM red-team |
| **v58 Stagehand** | Classroom + cohort + instructor mode |
| **v59 Doublecross** | FedRAMP Moderate control map + daily ConMon |
| **v60 Sun & Salt** | SBOM drift detector + IPO readiness self-test + external blocker playbook |

Some of these features are master-internal — the codesprint shipped capability across all three images, but the surface visible in each varies by license tier. The public ISOs (GRIMOIRE Public + Goodlife) carry their full intended share of the work.

---

## imminent — public ISO releases

The work toward public distribution is in flight.

- **GRIMOIRE Public ISO** — the gamified training platform, signed with cosign, anchored in Rekor, distributed publicly. First-boot wizard, faction selection, 100-lab corpus, full game engine, integrity-manifest enforcement.
- **Goodlife ISO** — the AI research variant. Jupyter, ALFRED `research-mode`, post-quantum experimentation toolkit, LUKS-encrypted research data.
- **Cohort program v1** — multi-tenant GRIMOIRE deployments for classes, clubs, and security teams.
- **Public Sigstore + Rekor** — verifiable supply chain from build oracle to USB stick.
- **Hive expansion playbook** (Stoneglass GA) — public Ansible recipe for self-hosting the 8-node Arcanum Hive.

These are not "someday" items. They're what the team is heading into next.

---

## near-term themes

**Tightening what exists.** The platform has been evolving fast. The next chapter sands every rough edge — onboarding, documentation, error messaging, first-boot polish, the unglamorous work that makes the user-visible improvement.

**Deeper AI augmentation.** ALFRED does its job today. There's a long list of ways it could do more — context, anticipation, usefulness in the operator's actual loop. v61–v65 carries that work forward.

**Continual GRIMOIRE content waves.** New labs. New boss contracts. New narrative arcs. New factions, possibly. Cohort tooling, definitely. The world deepens with every release.

**Mesh, made easier.** Distributed-by-default sounds simple in a sentence and is harder in practice. We're working on the parts that make a mesh feel inevitable rather than effortful.

---

## medium-term — the v61–v70 horizon

Themes we're paying attention to, in rough priority order:

- **Public release cadence** — predictable, signed, transparent. ISOs every cycle.
- **Cohort programs at scale** — clubs, classes, training programs running on shared GRIMOIRE infrastructure.
- **AI capability ladder** — bigger models, smarter routing, deeper integration with the kernel observability surface.
- **Reproducible builds in production** — every public ISO byte-for-byte reproducible by an independent verifier.
- **Federation between independent operators** — Hive-to-Hive, with cryptographic identity and permissioned visibility.
- **Curriculum partnerships** — formal mappings between GRIMOIRE progression and academic / industry training.
- **Hardware diversity** — supported architectures beyond x86_64.
- **Mobile companion** — read-only operator dashboard for on-the-go awareness.

Specific version numbers attach to specific deliverables as we get closer. Today's roadmap is themes; tomorrow's commit log is the truth.

---

## long-term — the north star

The end-state we're moving toward is a platform where the operator owns their infrastructure, their intelligence, and their future — not in a slogan, but **mechanically, cryptographically, architecturally**. The pieces are there. The work is in fitting them together with the polish, the trust, and the longevity that an operating system deserves.

We are not building a product. We are building **infrastructure for sovereignty**, with the long-term operator community in mind.

The roadmap reflects that.

---

## what isn't on this roadmap

The Operator (Master) image's internal feature trajectory. It exists. It evolves alongside the public roadmap. It is not for public distribution and is not part of this document by design.

If a master-internal capability ever crosses the boundary into a public image, it shows up here.

---

## how to follow

The work happens in public, in this repository's metadata and in the cadence of releases. Watch this repo. When the chapters change, the documents change with them.
