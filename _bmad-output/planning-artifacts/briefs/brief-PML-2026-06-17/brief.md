---
title: "Product Brief: PML (PredictionMarketLitigation)"
status: final
created: 2026-06-17
updated: 2026-06-17
---

# Product Brief: PML (PredictionMarketLitigation)

> The open, data-driven source of record for U.S. prediction-market litigation — and a public, working demonstration of trustworthy autonomous AI. *Built by AI, governed and approved by a human; corrections welcome.* Depth and downstream detail live in `addendum.md`; decisions and rationale in `.decision-log.md`.

## Executive Summary

PML is two things at once: the open, data-driven source of record for the fast-moving U.S. prediction-market litigation — Kalshi, Polymarket, Robinhood, the CFTC, and the states — and a public, working demonstration of how to build *trustworthy* autonomous AI. A fleet of AI agents scours primary legal sources daily and drafts case-law and regulatory updates, a state-by-state status map, a circuit-split heat map, and a Supreme-Court certiorari-likelihood signal. Nothing publishes until a human — the founder, an attorney — approves it. Every run passes through a documented nine-layer AI-governance stack (gateway, guardrails, action policy, orchestration, identity, observability, lineage, evals, GRC), and the evidence of each run — trace, lineage, eval scores, dollars spent, even where two agents disagreed — is exposed publicly at `ops.`.

The litigation is the subject; the governance is the message. The entire build is narrated in public, in the founder's voice, as a milestone-triggered journal that walks readers up that same nine-layer model — turning a niche legal tracker into portfolio-grade proof that one person can architect autonomous AI you can actually trust. Why now: the circuit split is crystallizing and a cert petition is imminent in summer 2026, so the story changes weekly — while the AI-governance field is loud, unsettled, and starved for a concrete, honest, open reference implementation.

## The Problem

**Two gaps, one project.**

*For anyone tracking prediction-market litigation:* the story moves faster than any single source keeps up with, and it's scattered. The core question — whether event contracts are CFTC-regulated "swaps" or state-regulated "wagers" — now spans 18+ states, four federal circuits, an imminent SCOTUS cert petition, a 267-page CFTC rulemaking, and a dozen bills. Litigators, compliance teams, traders, and journalists reassemble it from BigLaw alerts (deep but sporadic), gambling trade press (fast but shallow), and a paywalled compliance tracker. No free source combines doctrinal rigor with daily cadence and quantitative signals about where this is heading.

*For anyone trying to trust autonomous AI:* "AI governance" has become marketing noise — a hundred tools, new acronyms weekly, no agreement on what the phrase even means. There is little public, end-to-end proof of an autonomous system that produces *published, consequential* output — legal analysis, no less — with real guardrails, human checkpoints, full traceability, and an honest accounting of what went wrong. The field is rich in frameworks and promises and short on receipts.

## The Solution

PML closes both gaps with one system.

A scheduled fleet of AI agents runs daily at **noon ET**, pulling from primary legal sources — court dockets, the Federal Register, regulatory filings, legislative trackers — to detect and draft what's new: case updates, a state-by-state status map, a circuit-split heat map, and a cert-likelihood signal. Every draft enters a **human-in-the-loop queue**; the founder, an attorney, reviews and approves before a word goes public. Each run flows through the nine-layer governance stack, and the evidence — trace, data lineage, eval scores, budget spent, and any inter-agent disagreement — is published openly at `ops.` (the project's live Crust layer).

Running alongside the machine is the human: a milestone-triggered **build journal**, in the founder's voice, narrating the construction layer by layer and — just as candidly — at the fault lines where things break. It lives canonically on-site, each post carrying the actual governance trace behind it, and syndicates outward for reach. The whole project is open source, end to end, so the promise isn't "trust me" — it's "here's everything; check the receipts, and tell me where I'm wrong."

## What Makes This Different

Trackers for this litigation already exist — so the edge is not "first to cover it." It's four things existing coverage doesn't combine:

- **An open, free data layer.** A circuit-split heat map, a state-by-state status map, and a cert-likelihood signal — visual and quantitative, not just narrative. Today's trackers are either narrative-only (and free) or rigorous (and paywalled); none give this away.
- **Radical transparency.** The system shows its work: open-source code, public run traces, data lineage, eval scores, and budget at `ops.`. It is AI-built and says so — and *invites correction*. "Here's everything; tell me where I'm wrong" turns readers into a distributed check on the machine, and makes the trust claim verifiable instead of asserted.
- **Rigor at cadence.** Real doctrinal depth — the CEA/"swaps"/preemption substance — delivered daily. It bridges the gap between slow-but-deep BigLaw alerts and fast-but-shallow trade press.
- **The unfair advantage is the founder.** A practicing attorney who is also a CTO — the rare combination that can write the doctrine *and* engineer the governance. This is the honest moat: execution plus a positioning almost no one else can occupy.

## Who This Serves

**Primary — the people who could hire or partner with the founder** (serves the #1 goal): CTOs, engineering and AI-governance leaders, prospective employers and clients. They come for the governance showcase, the `ops.` receipts, and the build journal — and leave convinced one person can build autonomous AI worth trusting.

**The domain audiences** (serve the #2 goal — cited authority):
- **Litigators** (gaming, fintech, appellate, preemption) tracking the docket.
- **Compliance & legal teams** at exchanges and brokerages needing state-by-state go/no-go — the most monetizable readers.
- **Traders & quants** watching how legal events move prices.
- **Journalists** wanting a citable, canonical timeline; **academics & regulators** wanting structured, neutral data.

The two audiences reinforce each other: the governance crowd validates *how* it's built, the legal crowd validates *what* it says — and each lends the other credibility.

## Success Criteria

PML succeeds when it is **public, useful, and visibly trustworthy** to the two communities it serves — people who care about AI governance and people who follow prediction-market litigation. Targets below are directional starting points, to be tightened as the project finds its footing.

**Reach & visibility** *(the headline)*
- Live and fully open source from day one — site, `ops.` dashboard, and repository all public.
- The build journal ships its complete **nine-layer series** and circulates in the AI-governance community (reads, shares, repo engagement).
- Discoverable: first-page ranking for core prediction-market-litigation queries within the first few months, with steady growth in readers.

**Authority & usefulness**
- Referenced or cited by others in either community — a journalist, a law-firm post, an academic, or a fellow practitioner links to it.
- The community engages the openness: issues, discussions, and *corrections* submitted — the invited human check working in public.

**Trustworthiness — the thesis, proven**
- Daily updates run reliably, with human approval before every publish.
- A low, transparently-handled correction rate — mistakes caught and fixed in the open.
- Agent activity and spend stay visible and bounded; the project demonstrably governs its own agents.

**Sustainability**
- Ads and donations trend toward covering monthly AI and infrastructure cost — the project pays for itself over time.

## Scope

**Guiding principle: launch thin, build in public.** Because the build *is* the story, PML should go live before it is "finished" — the unbuilt layers become the journal's material. v1 is the thinnest system that proves the thesis end to end, in the open.

**In for v1 (launch):**
- **Public site** with the litigation tracker — a state-by-state status map and a circuit-split heat map, seeded from existing research and kept current.
- **One daily agent pipeline** (noon ET) monitoring primary sources (e.g., CourtListener, Federal Register) → drafts updates → **human-in-the-loop approval** → publish.
- **Governance spine instrumented and visible:** AI gateway with budget caps, tracing + evals, human approval, and data lineage — not all nine layers perfected, but the backbone real and observable.
- **`ops.` dashboard** — runs, traces, eval scores, budget spent, and approval decisions, public.
- **Build journal** — launched, first post(s) live, canonical on-site.
- **Open-source repo public** — issues + discussions on, correction invitation, "not legal advice" disclaimer, "Powered by Bizmation," "Buy Me a Coffee."

**Explicitly out of v1 (built in public, later):**
- The market-derived cert KPI from Kalshi/Robinhood (data sourcing unresolved — launch with a clearly-labeled qualitative signal instead).
- Ads (no traffic to monetize yet; revisit alongside the neutrality trade-off).
- Full maturity of all nine governance layers; inter-agent-disagreement visualizations.
- Programmatic SEO at scale and multiple content pillars.
- Anything that delays a first honest, governed, end-to-end publish.

**Later phases:** market-derived KPI once data access is sorted → remaining governance layers → agent-disagreement views → ads when traffic warrants → SEO scale.

## Risks & Constraints

- **Data access (gating).** Kalshi's data terms restrict AI/ML use and redistribution; Robinhood's automated-access terms are also restrictive. The market-derived cert KPI depends on resolving licensed or permitted access — which is why it sits outside v1.
- **Legal exposure.** Publishing legal analysis carries unauthorized-practice-of-law and defamation considerations. Mitigated by an information-only (not advice) posture, clear disclaimers, neutral sourcing to primary documents, and — structurally — human approval before every publish.
- **Accuracy *is* the product.** Because the content is AI-drafted, one confident error erodes the entire trust thesis. Human-in-the-loop review, transparent corrections, and public traces are the controls — and they have to actually work.
- **Neutrality vs. revenue.** Ads — especially from covered exchanges — conflict with the neutral-authority positioning. Deferred until traffic justifies the trade-off, and taken consciously when it comes.
- **Naming.** "Prediction" vs. "Predictive" is currently inconsistent across the domain, repo, and references. One canonical name must be chosen before public launch.
- **Solo and out-of-pocket.** One person, real costs. Bounded budgets with visible alerts are a hard requirement, not a nicety — a runaway agent is both a financial and a credibility risk.

## Vision

In two to three years, PML is the reference others reach for in *both* of its worlds: the canonical, trusted record of prediction-market litigation, and the open blueprint people cite when they ask what governed, trustworthy autonomous AI actually looks like in production.

The engine is the deeper bet. The nine-layer governed pipeline is domain-agnostic — today it tracks one fast-moving legal fight; the same open framework could track any evolving, high-stakes domain. PML is the first instance of a reusable pattern, not a one-off site.

And even if the litigation resolves — the Supreme Court rules, the question settles — PML's archive stands as the definitive contemporaneous history of how it unfolded, and the governance framework outlives the topic that proved it.
