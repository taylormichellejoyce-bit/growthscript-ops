# GrowthScript Framework

GrowthScript is ASG's messaging playbook — a value-first content accelerator that defines, aligns, and scales how your company tells its story.

This guide explains the framework and how to operationalize it with Claude Code.

---

## What GrowthScript Is

GrowthScript has two phases:

1. **Codify** - Create the foundational messaging components (the "single source of truth")
2. **Activate** - Use AI to generate assets from that foundation

The framework itself is excellent. What we're evolving is *how* you activate it.

---

## Phase 1: Codify

Codify is where you build the building blocks. There are four main components:

### 1. Product Language Guide

Defines *what the product is* in clear, factual language. Not marketing speak — structure and clarity.

**The hierarchy:**

| Level | Definition | Unit of Sale? |
|-------|------------|---------------|
| **Company** | The brand/business entity | No |
| **Platform** | Shared technology foundation (if products are unified) | No |
| **Portfolio** | Complete set of products offered | No |
| **Product** | Named offering, basis for contracts and pricing | Yes |
| **Capability** | Functional grouping of features that enables an outcome | Sometimes |
| **Feature** | Specific tool/function that delivers a discrete action | No |

*"Unit of Sale" = Can customers actually purchase this? Products are what appear in contracts and have pricing. Capabilities are sometimes sold separately as add-ons or edition upgrades. Everything else is organizational structure, not something you sell.*

**What to document for each product:**
- Product overview (what it is, who buys it, who uses it)
- Packaging/editions (if applicable)
- Capabilities (outcome-oriented groupings)
- Features (parity vs. differentiating)

**Key principle:** Product Language is *descriptive, not persuasive*. It tells you what exists and how it's organized — not why it matters.

---

### 2. ICP + Personas

Defines *who you serve* and how they buy.

**ICP (Ideal Customer Profile):**
The type of organization you're built to serve.

Document:
- Industry/vertical
- Size and complexity (revenue, employee count, locations)
- Geography and footprint
- Regulatory/risk profile
- Technology maturity
- Buying triggers and readiness signals
- Disqualifying factors

**Personas:**
The people who influence, buy, and use your products.

For each persona, document:
- Typical titles
- Role summary
- Buying role (see below)
- Goals and success metrics
- Main pains and risks
- What they care about in evaluation
- How they interact with your product

**Buying Roles:**

| Role | Definition |
|------|------------|
| **Champion** | Feels the pain, drives the buying process end-to-end |
| **Economic Buyer** | Controls budget, grants final approval |
| **Influencer** | Shapes decision through expertise or credibility |
| **Technical Approver** | Validates integration, security, compliance |
| **Implementor** | Manages setup and rollout |
| **User** | Engages day-to-day, feedback drives renewals |

One person may serve multiple roles.

---

### 3. Core Messaging Components

Articulates *what you are* and *the value you deliver*. This is the strategic foundation for all communication.

**Category Strategy:**
- What market/category do you compete in?
- Category name and definition
- "Why now" narrative (market shifts, pressures)
- Legacy approach vs. new evaluation criteria

**Platform Strategy** (if applicable):
- How products work together as a system
- Shared data, workflows, intelligence
- Why the integrated model matters

**Leadership Claim:**
- What you can credibly claim to lead
- Why customers should choose you
- Proof points that back it up

**Messaging Pillars:**
3-5 enduring truths that define your value. Each pillar:
- Has a name and summary
- Connects persona pains to capabilities to outcomes
- Is supported by proof points

**Positioning Statements:**
- Company-level positioning (ICP + category + leadership + pillars)
- Product-level positioning (1-2 sentences per product)
- Any "locked" copy that must be preserved

**Competitive Landscape:**
- Direct competitors
- Category-level alternatives
- Status quo (spreadsheets, manual processes)
- How you're different

---

### 4. Jobs To Be Done (JTBD)

Documents what each persona is *trying to accomplish* and how your product enables it.

**JTBD format:**
> "When [situation], I want [motivation], so I can [desired outcome]."

**JTBD Supertable columns:**

| Column | What It Captures |
|--------|------------------|
| Job To Be Done | The outcome-oriented statement |
| Metrics/KPIs | How success is measured |
| Pain Points/Blockers | What makes the job hard today |
| Current Way | How they do it without you (manual, legacy tools) |
| Product Alignment | Your product/capability that enables the job |
| Use Cases | Concrete workflows where this happens |
| Proof Points | Evidence of improvement (stats, quotes) |

Create a JTBD supertable for each primary persona, organized by their 4-6 core responsibilities.

---

## Phase 2: Activate

This is where the original GrowthScript playbook and the Claude Code approach diverge.

### The Original Method (ChatGPT Era)

1. Gather source materials (decks, docs, transcripts)
2. Convert everything to markdown
3. Upload to ChatGPT with the CODIFY Assistant prompt
4. Get the structured framework output
5. Paste into your "[Company] Framework" doc
6. Clean up [GAP], [ASSUMPTION], [CONFLICT] tags
7. Create a custom GPT with your framework as Knowledge
8. Copy/paste prompts to generate assets
9. Copy/paste outputs to your tools

**The problem:** You become the middleware. Every update flows through you manually. When things get busy, the framework drifts.

### The Claude Code Method

1. **Connect your sources** - Link Claude Code to Notion, Linear, Slack via MCP
2. **Establish your source of truth** - Build your GrowthScript framework in Notion
3. **Work together** - Claude reads from your sources, writes to your tools
4. **Stay current** - Updates happen where work happens, not in a separate GPT

**The difference:**

| ChatGPT Era | Claude Code Era |
|-------------|-----------------|
| Copy context in, copy output out | Claude reads and writes directly |
| You paste between tools | Claude works inside your tools |
| Framework lives in a GPT Knowledge file | Framework lives in Notion (your source of truth) |
| Updates require manual sync | Updates happen in real-time |
| You are the middleware | Claude is your partner |

---

## Building Your GrowthScript

### If Starting Fresh

**Week 1-2: Foundation**
- Define Product Language hierarchy
- Draft ICP definition
- Identify primary personas

**Week 3-4: Messaging**
- Develop category strategy
- Craft leadership claim
- Define messaging pillars
- Write positioning statements

**Week 5-6: JTBD + Activation**
- Build JTBD supertables for each persona
- Set up your Notion structure
- Connect Claude Code to your tools

### If You Have Existing Materials

1. Connect Claude Code to where your docs live
2. Ask Claude to help you audit what you have vs. what you need
3. Fill gaps systematically using the framework structure
4. Consolidate into your source of truth

---

## Handling Gaps and Assumptions

When building your framework, you'll encounter missing information. Use these tags:

- **[GAP]** - Critical information is missing (e.g., "[GAP] No clear packaging tiers defined")
- **[ASSUMPTION]** - You're inferring something obvious (e.g., "[ASSUMPTION] Primary users are regional managers based on case studies")
- **[CONFLICT]** - Sources disagree on something

Be aggressive about surfacing gaps. It's better to flag what's missing than to quietly guess.

---

## Resources

- [GTM Functions](gtm-functions.md) - Key PMM activities and workflows
- [Getting Started](../guides/getting-started.md) - Terminal setup for beginners

---

## Credits

GrowthScript was developed by ASG (Alpine Software Group) as a PMM playbook for portfolio companies. This guide documents the framework and extends the activation methodology using Claude Code.
