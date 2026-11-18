# Open-source ecosystem readiness: ICN, Mutualware, and NYCN

> **Status:** DRAFT PROPOSAL for maintainer and institutional review (2026-11-17).
> **Scope:** Public coordination and publication criteria, not an adoption decision, roadmap override, release claim, or authorization to publish private sources.
> **Authority:** Individual repositories and legitimate institutional bodies remain the source of truth. This document is a navigation and planning aid only.

## Goal

Make three related efforts discoverable, reproducible, welcoming, secure, and genuinely contributor-maintainable without turning democratic infrastructure into a single administrator-controlled project.

**Open source is not equivalent to making every repository public.** Source code, instructions, public decisions, fixture data, and tests should be reproducible and open wherever lawful and safe. Credentials, personal information, real organizational records, unpublished institutional decisions, and operational secrets must remain private.

## Distinct domains and boundaries

| Domain | Purpose | Current verified GitHub footing | Boundary |
| --- | --- | --- | --- |
| **ICN** | Generic, interoperable institutional protocol/runtime: identity, scoped authority, governance, evidence, resource coordination, and federation | [InterCooperative-Network/icn](https://github.com/InterCooperative-Network/icn) public | Must not hardcode NYCN-specific decisions into generic primitives |
| **Mutualware** | Working name for reusable human-facing cooperative software, providers, adapters, and public software commons | No separate repository in this GitHub organization observed on 2026-11-17 | Product/brand/repository boundaries remain **proposed**; do not assert established software or deployment |
| **NYCN** | Independently governed New York cooperative network and its institution-specific applications and programs | [InterCooperative-Network/nycn](https://github.com/InterCooperative-Network/nycn) private | Institutional authority stays with NYCN; publisher/developer permissions are not governance rights |

**Existing identity work:** [ICN #2801](https://github.com/InterCooperative-Network/icn/issues/2801) proposes a Mutualware public-brand transition and protects technical compatibility. Reconcile that proposal with the three-project open-source model before declaring a new canonical public brand or splitting implementation. Do not bulk rename `icn-*`, `icnd`, `icnctl`, `did:icn:*`, wire formats, crypto strings, release links, or historical records.

**Preserve current facts:** ICN is substantial but not a verified production-ready institutional federation. NYCN's repository is a development/rehearsal package, not proof of formal adoption or a live production pilot. Public artifacts must distinguish planned, implemented, tested, deployed, and institutionally accepted.

## Shared minimum open-source standard

Each independently published software repository should provide:

1. **Identity and scope:** README that answers what it is, who it serves, what's actually working, what it is not, and how it relates to the other projects.
2. **Legal clarity:** recognized OSI-compatible license, copyright/provenance audit, third-party notices where needed, and explicit license scope. ICN and NYCN already contain GNU AGPLv3 license files; do not replace those by default.
3. **First contribution:** practical `CONTRIBUTING.md`, a working quickstart, development commands that a clean machine can run, good-first-issue examples and noncoding contribution paths.
4. **Community health:** code of conduct with a real enforcement contact/process; private security reporting; transparent support and maintenance expectations; issue/PR templates.
5. **Engineering:** tagged releases, changelog, compatible versioning, CI that tests from clean checkout, reproducible fixture/example environments, dependency/license scanning, and provenance for artifacts. State failures honestly.
6. **Decision-making:** written distinction between project maintainers, reviewers, contributors, participants, elected or delegated institutional decision-makers; transparent proposal/decision/appeal/maintainer onboarding process.
7. **Sovereignty:** independently hostable services where applicable; documented configuration, upgrades, data export, restore, key management and ownership boundaries. A public GitHub repository is not an independent deployment by itself.
8. **Participation:** documentation/design/accessibility/testing/research routes, regular triage and mentor support without credential-based gatekeeping; clear acknowledgements and non-pay-to-vote contribution rules.
9. **Operational honesty:** project-level readiness/status record backed by repository-specific evidence; never copy stale status assertions from an umbrella registry.

Favor links to existing authoritative files rather than maintaining conflicting copies. Do not invent governance votes or institutional endorsements.

## Project-specific workstreams

### ICN — improve an existing public project

- **Preserve existing assets.** README, AGPLv3 license, CONTRIBUTING, CODE_OF_CONDUCT, SECURITY, GitHub issue forms, architecture and onboarding documentation already exist on `main`.
- Reconcile and test the contributor-first onboarding draft [PR #2825](https://github.com/InterCooperative-Network/icn/pull/2825) and its [newcomer walkthrough #2826](https://github.com/InterCooperative-Network/icn/issues/2826) before duplicating those changes.
- Draft a **technical project governance/maintainer process** (who may merge, how to become a maintainer, conflict handling, security exceptions, release responsibility), explicitly distinct from protocol-level or institutional governance.
- Audit current release artifacts, installation instructions, CI health, security advisories, dependency licenses, and supported platforms before publishing a stable support promise.
- Curate bounded starter issues for Rust, TypeScript, docs, testing, accessibility and cooperative-domain review.

### Mutualware — establish a public project without erasing ICN

- First publish a reviewed scope statement: reusable apps, service contracts, adapters, composable user interfaces and commons work; identify the smallest **actually implemented** portable capability to publish with tests and documentation.
- Resolve #2801 brand/project ambiguity and GitHub namespace/domain control with human review. Until then, call it a proposed project/brand and retain ICN compatibility surfaces.
- Choose public repository/org layout only after inventorying existing code ownership and Git history. Avoid a giant code migration or an empty marketing repo labeled a ready platform.
- Start with one clean, fixture-driven, independently runnable example plus a versioned contract, contributor quickstart and a public technical roadmap. Do not publish provider credentials or internal infrastructure.
- Prefer extraction prompted by at least two genuine consumers over speculative frameworks.

### NYCN — publish software, not institutional/private data

- **Do not flip the existing private `nycn` repo to public.** Its complete history, PR discussions, logs, author metadata, fixtures and links require a separate publication review. GitHub visibility changes can expose Actions history/logs.
- Establish NYCN's human-approved publication and code-custody policy: what is publishable, who may approve it, which records require consent, and who maintains the resulting public package.
- Prepare a **clean public software release** from reviewed files on a fresh public repository/history or an approved code-only package; publish fictional fixtures, generic schemas, tests, safe architecture and setup instructions. Do not carry private Git history by default.
- Preserve private operational sources, contact details, unpublished governing decisions, personal data, credentials, meeting transcripts, access tokens, non-public URLs, and private host topology. Test negative examples, including built/browser assets.
- Integrate existing Organizer Home direction [NYCN #113](https://github.com/InterCooperative-Network/nycn/issues/113) and publication-discipline [PR #141](https://github.com/InterCooperative-Network/nycn/pull/141); neither proves public readiness or institutional adoption.
- Publish a fully fictional year/program example and one reproducible organizer workflow. Keep real-world assignments, approvals, and evidence behind human-reviewed authority boundaries.

## Safe launch sequence (gates, not calendar promises)

**Gate A — inventory and publication safety**
- [ ] Record canonical repo/package owners, license/provenance, code/history sensitivity, dependencies and outstanding branches/PRs.
- [ ] Identify existing docs and policy work to reuse; create no overlapping ownership registry.
- [ ] Designate a human reviewer for any private-to-public movement and an institutional approver for NYCN content.

**Gate B — contributor experience**
- [ ] Newcomer can find a task, clone the exact repository, run a documented check, submit a change, and receive review.
- [ ] Each repository has a real security channel, code of conduct and transparent maintainer path.
- [ ] Public status says exactly what's implemented, what is rehearsal-only, and what still needs institutional acceptance.

**Gate C — useful reproducible output**
- [ ] ICN has an externally verified quickstart and documented tagged/reproducible release path.
- [ ] Mutualware has at least one useful, runnable, separately scoped public component, not only a concept page.
- [ ] NYCN has a publication-approved, fictional-data runnable example with independent privacy tests.

**Gate D — durable community**
- [ ] Triage ownership, response expectations, release cadence and decisions/appeals are maintained openly.
- [ ] Contributions can be made without joining a private organization, purchasing influence, or running the whole stack.
- [ ] Independent deployment, exit, export/recovery and fork paths have been tested, not merely asserted.

## Recommended immediate delivery lanes

- **ICN Core:** verify and land existing newcomer guidance when ready; propose maintainership and release criteria separately.
- **Mutualware:** public scope/contract inventory, compatibility decision, first reusable fixture-backed extraction.
- **NYCN:** private publication inventory and approved clean public package; do not change visibility.
- **Community/Public:** cross-project front door linking to canonical status, contribution routes and real starter tasks.
- **Infrastructure:** CI, security, SPDX/SBOM/provenance where appropriate, reproducible release packaging, independent deployment tests.

Development sessions/worktrees are temporary execution contexts, not project authority. Tie work to named lanes, reviewed branches, verified PRs and repo-owned truth; do not let a TUI, AI agent, or website redefine governance or release status.

## Decisions still needing explicit review

- Is Mutualware the public umbrella/brand for the ICN lineage, a distinct reusable software project, or both with documented boundaries? Reconcile with ICN #2801.
- Who legitimately approves NYCN public code releases and institution-specific representations?
- What is the initial Mutualware canonical repository/namespace and first real extracted package?
- What maintains technical project governance versus NYCN member governance?
- Which release/support levels can be claimed today based on reproducible evidence?

**Non-goals:** no repository visibility change; no production DNS/domain migration; no unsolicited publicity; no license replacement; no merging existing feature stacks; no synthetic claim of elected authority, production deployment, or project maturity.
