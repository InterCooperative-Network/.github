# InterCooperative Network

ICN is institutional infrastructure for democratic organizations. It is being built so cooperatives, communities, and federations can prove decisions, operate on infrastructure they control, and coordinate across organizational boundaries without handing those functions to a platform landlord.

**Public site:** [intercooperative.network](https://intercooperative.network)

## What ICN is

A constraint engine, not a blockchain and not a federated SaaS. Apps translate cooperative governance into generic constraints; the kernel enforces those constraints without understanding their meaning. This is what keeps the substrate predictable while letting cooperatives adapt the rules above it.

The substrate covers identity, trust, networking, mutual-credit accounting, contracts (CCL), gossip, governance, and trust-gated compute.

For the longer answer, start with [What is ICN](https://intercooperative.network/what-is-icn) and [What's Real Now](https://intercooperative.network/whats-real-now).

## Repositories

| Repo | Visibility | Role |
|---|---|---|
| [`icn`](https://github.com/InterCooperative-Network/icn) | **Public** | Canonical substrate. Kernel, apps, daemon, CLI, gateway, TypeScript SDK, public website. The truth lives here. |
| [`nycn`](https://github.com/InterCooperative-Network/nycn) | Private | NYCN — first institution-specific application package built on ICN. |
| [`icn-learn`](https://github.com/InterCooperative-Network/icn-learn) | Private | ICN Academy — role-based learning and onboarding. |
| [`icn-community-bridge`](https://github.com/InterCooperative-Network/icn-community-bridge) | Private | Discord-to-Matrix bridge — scaffold/docs only, not deployed. |

Public claims are grounded in the [`icn`](https://github.com/InterCooperative-Network/icn) repo. NYCN and icn-learn are private while they mature; their pieces become public as they get pilot-ready.

## Where things live

- **Roadmap and current state:** [`docs/STATE.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/STATE.md), [`docs/PHASE_HISTORY.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/PHASE_HISTORY.md), [`docs/dev-journal/ROADMAP.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/dev-journal/ROADMAP.md). State files are bumped with every state-changing PR.
- **Architecture:** [`docs/ARCHITECTURE.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/ARCHITECTURE.md) and [`docs/architecture/`](https://github.com/InterCooperative-Network/icn/tree/main/docs/architecture).
- **Cross-repo navigation:** [`docs/reference/project-index/repository-map.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/reference/project-index/repository-map.md).
- **Public discussion:** [GitHub Discussions](https://github.com/InterCooperative-Network/icn/discussions). Conversation belongs in Discussions; decisions belong in issues, PRs, RFCs, and ADRs.

## How to contribute

- **Read the project first:** [intercooperative.network/get-involved](https://intercooperative.network/get-involved).
- **Technical contributors:** [`docs/GETTING_STARTED.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/GETTING_STARTED.md), then [`CONTRIBUTING.md`](https://github.com/InterCooperative-Network/icn/blob/main/CONTRIBUTING.md). For a first contribution, browse [good first issues](https://github.com/InterCooperative-Network/icn/issues?q=is%3Aissue+is%3Aopen+label%3Agood-first-issue).
- **Non-technical contributors:** docs, design, testing, research, policy, and ecosystem paths are listed on [Get Involved](https://intercooperative.network/get-involved).
- **Cooperatives evaluating ICN as substrate:** open a [Discussion](https://github.com/InterCooperative-Network/icn/discussions) once the use case is concrete.

## Security

**Do not file vulnerabilities as public issues.**

Report through [GitHub's private vulnerability advisory flow on `icn`](https://github.com/InterCooperative-Network/icn/security/advisories/new). Full policy in [`SECURITY.md`](https://github.com/InterCooperative-Network/icn/blob/main/SECURITY.md).

## What is not production-ready

ICN is **pre-pilot**. The substrate has working kernel, identity, trust, gossip, ledger, governance, and gateway, deployed on a K3s cluster for live testing — but pilot deployment is the next phase, not a current capability. The [`docs/security/`](https://github.com/InterCooperative-Network/icn/tree/main/docs/security) directory and [`docs/STATE.md`](https://github.com/InterCooperative-Network/icn/blob/main/docs/STATE.md) are candid about which surfaces are hardened and which are still research-grade.

Public claims on the website distinguish "What's Real Now" from direction. If you are evaluating ICN for an institutional use case, start there.

## Support the work

The current rail is [GitHub Sponsors](https://github.com/sponsors/InterCooperative-Network). Sponsorship supports development; it does not grant governance authority, roadmap influence, or private access to maintainers.

---

This is an organization profile. For the day-to-day project, start in [`icn`](https://github.com/InterCooperative-Network/icn).
