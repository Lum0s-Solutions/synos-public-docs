# GRIMOIRE

### *the gamified cybersecurity training platform that ships as the public face of Syn_OS.*

---

## the premise

Most cybersecurity training looks like this: read a chapter, watch a video, do a sandbox exercise, take a quiz, repeat. Linear. Disconnected. Optimized for completion, not for fluency.

GRIMOIRE rejects all of that.

GRIMOIRE is a **world**, not a curriculum. You enter as a novice. You leave as someone who's lived through scenarios that actually happened to people, with consequences that actually mattered, in factions whose loyalties you actually felt.

It's the platform we ship to the community. It's the closest thing we know how to build to *learning by doing it for real, with everything that implies.*

---

## by the numbers

| | |
|---|---|
| Hand-authored labs | **100**, exact (enforced by integrity manifest) |
| Lab categories | **13** (beginner, advanced, crypto, web, network, forensics, reversing, ai-red-team, ad, cloud, mobile, hardware, osint) |
| Certification paths mapped | **11** (CompTIA Security+ / CySA+ / PenTest+, OSCP, OSWE, CRTP, CRTO, CEH, CISSP foundations, GIAC GPEN/GCIH, eJPT) |
| Game engine plugins | **8** (cutscene, mindmap, retro filter, cyberspace, skill tree, faction HQ, rehoboam, twin) |
| Game-mode crates | ~110+ modules, ~53,000 lines of code |
| First-boot onboarding | **Wizard-driven**, faction selection, calibration, opening lab seed |

---

## the world

### factions

You pick a faction at the first-boot wizard. Each faction has a distinct relationship to power, secrecy, and what counts as ethical engagement. **Crimson Spire**, **Ashen Veil**, and the third house each shape what missions are on offer, who you can trust, what equipment opens up, and how cohorts measure each other's worth across server walls.

There are no "good guys" and "bad guys." There are people with different philosophies, and you've chosen one. Faction reputation gates content. Allegiance shifts have costs. Inter-faction wars are a recurring narrative beat.

### labs

The atom of progression is the **lab** — a hand-authored challenge built around a specific technique, vulnerability, or defensive posture. The 100-lab corpus spans:

- **Beginner** (14 labs) — first-contact for users with no prior background.
- **Advanced** (14 labs) — hard multi-stage exploitation, real-world complexity.
- **Crypto** (6 labs) — classical and modern crypto attacks and misuses.
- **Web** — full-spectrum web application security, from XSS to deserialization to cache-deception.
- **Network** — protocol abuse, lateral movement, segmentation analysis.
- **Forensics** — disk, memory, network, timeline reconstruction.
- **Reversing** — static and dynamic analysis, anti-debugging, packers.
- **AI red team** (6 labs) — attacks on ML/AI systems and prompt-driven agents.
- **Active Directory** — kerberoasting, golden tickets, ACL abuse, BloodHound recipes.
- **Cloud** — AWS/Azure/GCP misconfiguration paths, IAM privilege escalation.
- **Mobile** — Android and iOS reverse engineering, runtime instrumentation.
- **Hardware** — embedded, firmware, side channel.
- **OSINT** — open-source intelligence and adversary attribution.

Every lab is real. Every solution is verifiable. Every credit is earned.

### boss contracts

Some scenarios are too big for a single lab. **Boss contracts** chain multiple labs into a single multi-stage arc — a piece of multi-week storytelling where you earn your way through stages, where partial progress matters, and where the final clear means something.

Boss contracts are the tests the system pulls out when it thinks you're ready.

### the economy

Earning is more than XP. GRIMOIRE has a **loot and crafting economy**. Solve labs, you earn artifacts. Combine artifacts, you craft equipment. Equipment opens doors. Better gear unlocks harder labs. Harder labs feed deeper missions.

It's not pay-to-win. It's *earn-to-play.*

### narrative quests

Threading through everything is a **branching narrative**. Quests with multiple paths. Choices that close some doors and open others. NPCs whose names you'll remember. Cutscenes that hit. A world with its own history before you arrived. You're not the protagonist — you're a new player in a world already in motion.

### cohorts and competition

GRIMOIRE plays best with peers. **Cohort mode** lets a class, a club, or a team compete on the same content. **Five competition modes** ship in the engine: leaderboard climbs, squad missions, faction wars, head-to-head challenge runs, and asymmetric red-vs-blue scenarios.

Some of the best labs can only be solved as a group.

---

## the path

GRIMOIRE is structured around a long arc: from **novice** to **operator**.

The early game is exploration. The middle game is mastery. The endgame is the **Sovereign Operator Path** — a curated sequence of challenges that graduates a player from "I can solve labs" to "I can run my own infrastructure, defend my own mesh, mentor others through the same arc."

Along the way, the system maps your progress against **11 established cybersecurity certification paths**. We don't replace certs. We make the practice that earns them feel like a story you're inside, not a syllabus you're slogging through.

---

## the first-boot wizard

The first time you boot Syn_OS, GRIMOIRE meets you with a wizard. It asks you what you're here for. What you already know. What scares you. What thrills you. It chooses a starting faction (you can override). It seeds a few opening labs. It puts you on a path that fits.

The wizard is not a personality test. It's a **calibration**. It tunes the early experience so the first hour doesn't waste you.

---

## lab integrity

Every lab in the 100-lab corpus is hashed and signed. The `INTEGRITY_MANIFEST.toml` at the root of the lab tree enforces: exact lab count, per-lab SHA-256, per-category counts. The build system refuses to publish an ISO whose lab corpus doesn't match.

This matters because GRIMOIRE is a training platform — the integrity of what you're being asked to learn is load-bearing. We don't ship if we can't verify.

---

## who it's for

- **Students** working through certification paths who want the practice to feel like something more than rote.
- **Self-taught practitioners** who want a structure without it feeling like one.
- **Cohorts and clubs** running their own programs and looking for a platform that scales with them.
- **Operators** who already know the craft and want a place to push apprentices through.
- **Security teams** running internal training cycles who want a real platform under the curriculum.

---

## what's coming

- **GRIMOIRE Public ISO release** — the platform, signed, downloadable, with the full first-boot experience.
- **Cohort program at scale** — multi-tenant deployments for clubs, classes, and corporate training programs.
- **Continual content waves** — new labs, new boss contracts, new narrative arcs, new factions over time.
- **Public Rekor-anchored releases** — verifiable signatures on every ISO.
- **Curriculum integrations** — partnerships with academic and industry training programs that map GRIMOIRE progression onto formal coursework.

The platform is the long game. Every release deepens the world.

---

<div align="center">

*every lab is a small death. every boss contract is a small rebirth.*

</div>
