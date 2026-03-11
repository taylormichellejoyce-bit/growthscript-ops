# GTM Functions for PMMs

Key activities and workflows for Product Marketing Managers operationalizing GrowthScript.

---

## The PMM Role in GTM

As a PMM, you sit at the intersection of:
- **Product** - What we're building and shipping
- **Marketing** - How we tell the story
- **Sales** - What they need to sell
- **Customer Success** - What customers need to succeed

Your job: Make sure everyone has accurate, current information about the product — and that GTM is ready *before* things ship, not after.

---

## When GTM Starts

**GTM does not start when something ships. It starts when your roadmap is locked.**

The moment your product team confirms what's being built, that's your trigger to begin GTM work. You build GTM in tandem with product — not as a handoff after the fact.

### A Note on Methodology

This guide uses language from **Shape Up** (Basecamp's product development methodology), where work is organized into cycles and "bets" are the projects committed for each cycle. "Bets are locked" = the roadmap is confirmed.

**Your organization may use different terms:**
| Shape Up | Scrum/Agile | Other |
|----------|-------------|-------|
| Cycle | Sprint/Quarter | Release train |
| Bets locked | Sprint committed | Roadmap finalized |
| Betting table | Sprint planning | Prioritization |
| Cooldown | Hardening sprint | Buffer |

**The principle is the same regardless of methodology:** Identify the moment when your org confirms what's being built, and start GTM there — not when things ship.

If you're unsure when that moment is, ask your product team: "When do you know for sure what's shipping this [cycle/sprint/quarter]?" That's your GTM start date.

```
Cycle bets are locked
        ↓
PMM assesses GTM needs for each project
        ↓
GTM work happens ALONGSIDE building
        ↓
By ship date: GTM is ready, not starting
        ↓
Release ships with GTM already in place
```

**Why this matters:**
- You have time to craft messaging, not rush it
- Sales enablement is ready on day one
- You can influence positioning while there's still time
- No scramble at launch

---

## Core GTM Functions

### 1. Release Tracking & Planning

**What it is:** Knowing what's coming and planning GTM in parallel with building.

**When to start:** The moment bets are confirmed for the cycle.

**Workflow:**
```
Product team confirms bets for cycle
        ↓
PM creates entry in Upcoming Releases (Status: In Progress)
        ↓
PMM triages: What GTM does this need?
        ↓
PMM begins GTM work in parallel with build
        ↓
GTM ready before ship (Status: Ready to Launch)
        ↓
Release ships (Status: Launched)
```

**What to track:**
- Project name and Linear link
- Release type (Feature, Enhancement, Bug Fix)
- Impacted teams (Sales, Support, Marketing, CS)
- Rollout scope (All customers, Enterprise only, Beta)
- Status (In Progress → Heads Up → Ready to Launch → Launched)
- GTM deliverables checklist

**Claude Code helps by:**
- Pulling Linear project details as specs evolve
- Summarizing technical changes for GTM messaging
- Flagging when projects are approaching ship date

---

### 2. Product Documentation

**What it is:** Keeping the "what does it do" docs accurate.

**When to start:** During the build, not after ship.

**Structure:**
```
Core Products
├── By Product
│   └── By Capability
│       └── Features + Details
└── Always current, always accessible
```

**Workflow:**
```
Bets locked for cycle
        ↓
PMM reviews Linear specs for upcoming features
        ↓
Draft doc updates based on planned functionality
        ↓
Refine as specs solidify during build
        ↓
Finalize docs before ship
        ↓
Publish when feature goes live
```

**The key shift:** Don't wait for "new feature ships" to start doc work. Start when you know what's being built.

**Claude Code helps by:**
- Reading Linear specs and PRDs as they evolve
- Drafting doc updates in your voice
- Finding existing docs that will need updates
- Tracking spec changes that affect your drafts

---

### 3. Sales Enablement

**What it is:** Arming Sales with what they need to sell.

**When to start:** When you know what's shipping and who it's for.

**Key deliverables:**
- Feature one-pagers
- Competitive battle cards
- Objection handling guides
- Demo scripts
- Pricing/packaging docs

**Workflow:**
```
New capability confirmed for cycle
        ↓
Assess: Does Sales need new enablement for this?
        ↓
Draft enablement during build phase
        ↓
Refine based on final specs
        ↓
Deliver to Sales BEFORE launch
        ↓
Train Sales so they're ready on day one
```

**Claude Code helps by:**
- Searching existing assets before creating new
- Drafting one-pagers from evolving specs
- Keeping competitive info updated

---

### 4. Launch Planning

**What it is:** Coordinating GTM activities for releases — planned in advance, not scrambled at ship.

**When to start:** When bets are locked.

**Tiers of launches:**
| Tier | What | GTM Effort | Lead Time |
|------|------|------------|-----------|
| Major | New product/capability | Full campaign, enablement, PR | Full cycle |
| Standard | Significant feature | Blog, email, sales training | 2-3 weeks |
| Minor | Enhancement/fix | Release notes, internal update | Days |

**Launch planning timeline:**
```
Bets locked (Cycle start)
        ↓
Week 1-2: Assess GTM tier, assign deliverables
        ↓
Week 2-4: Draft messaging, enablement, content
        ↓
Week 4-5: Refine based on build progress
        ↓
Week 5-6: Finalize, brief teams, prep launch
        ↓
Ship date: Execute launch (not start planning)
```

**Launch checklist (complete BEFORE ship):**
- [ ] Messaging finalized
- [ ] Sales enablement created and delivered
- [ ] Support documentation updated
- [ ] Marketing assets ready
- [ ] Internal teams briefed
- [ ] Customer communication drafted

**Claude Code helps by:**
- Pulling all relevant project context
- Drafting launch materials from specs
- Checking if all pieces are in place before ship

---

### 5. Competitive Intelligence

**What it is:** Understanding how you compare to alternatives.

**When to update:** Ongoing, plus before major launches.

**What to track:**
- Competitor positioning and messaging
- Feature comparison
- Pricing (if available)
- Win/loss patterns
- Market moves and announcements

**Workflow:**
```
Competitor announces something
        ↓
Document in competitive landscape
        ↓
Assess impact on your positioning
        ↓
Update battle cards if needed
        ↓
Brief Sales
```

**Also:** Before a major launch, refresh competitive positioning to ensure your messaging accounts for current landscape.

**Claude Code helps by:**
- Researching competitor updates
- Comparing feature sets
- Drafting battle card updates

---

## The Documentation Stack

Where things live:

| Doc Type | Location | Updated |
|----------|----------|---------|
| Core Products | Notion | During each cycle (not after ship) |
| Upcoming Releases | Notion | Continuously from bet lock to launch |
| Sales Assets | Notion/Drive | Ready before each release |
| Competitive Intel | Notion | Monthly + before major launches |
| GrowthScript Framework | Notion | Quarterly |

---

## Common PMM Pain Points

| Pain Point | Traditional Fix | Claude Code Fix |
|------------|----------------|-----------------|
| GTM is always rushed | "Ship then scramble" | Start at bet lock, build in parallel |
| Docs go stale | Manual audits after ship | Update during build, not after |
| Context scattered | Meetings, Slack, emails | Claude searches Linear/Notion |
| Same questions repeatedly | Answer ad-hoc | Claude finds existing answers |
| No time for everything | Prioritize ruthlessly | Claude handles routine updates |

---

## PMM + Claude Code Cadence

**At Cycle Start (Bets Locked):**
- Review all confirmed bets
- Assess GTM tier for each project
- Create Upcoming Releases entries
- Start GTM work for major items

**Weekly During Cycle:**
- Check Linear for spec updates on your projects
- Refine drafts based on build progress
- Update Upcoming Releases status
- Flag blockers or changes that affect GTM

**Pre-Ship (1-2 weeks before):**
- Finalize all GTM deliverables
- Brief Sales, Support, CS
- Stage marketing content
- Confirm launch checklist complete

**At Ship:**
- Execute launch (not start planning)
- Update status to Launched
- Publish docs and enablement
- Monitor initial reception

**Post-Ship:**
- Gather feedback
- Update docs if needed based on real usage
- Capture learnings for next cycle

---

## The Key Mindset Shift

**Old way:** Product ships → PMM scrambles → GTM happens late

**New way:** Bets lock → GTM starts → GTM ready when product ships

GTM is not a reaction to shipping. It's a parallel workstream that runs alongside building. When you treat GTM as something that happens *after* ship, you're always behind. When you start at bet lock, you're ready on day one.

---

## Getting Started

1. Get visibility into your product team's cycle planning
2. Set up your Upcoming Releases tracker
3. Connect Claude Code to Notion and Linear
4. Start with one cycle: plan GTM from bet lock, not ship
5. Iterate and expand

See [Getting Started Guide](../guides/getting-started.md) for setup instructions.
